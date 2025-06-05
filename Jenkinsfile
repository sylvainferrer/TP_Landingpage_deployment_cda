pipeline {
    
    agent none

    stages {
        stage('Git clone') {
            agent { label 'agent-lftp' }
            steps {
                git branch: 'main', url: 'https://github.com/sylvainferrer/TP_Landingpage_deployment_cda.git'
            }
        }
        stage('Copy server') {
            agent { label 'agent-lftp' }
            steps {
                sh '''
                   lftp -u lp-hoopstore,"$Mdp" "$ftp" -e "mirror -R ${WORKSPACE}/ www/ ; quit"
                '''
            }
        }
    }
}
