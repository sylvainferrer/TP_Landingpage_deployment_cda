# 🎧 PodcastZone - Landing Page

Cette landing page est conçue pour attirer l'attention des visiteurs et les inviter à vous contacter directement par email pour en savoir plus sur votre plateforme de podcasts.

---

## 🚀 Aperçu

- Interface responsive et animée en **HTML/CSS/JS pur**
- Bouton "Nous contacter" qui ouvre automatiquement le client mail de l'utilisateur (`mailto:`)
- Idéal pour collecter des leads sans base de données ni backend

## 📩 Modifier l'adresse email

Le bouton utilise un lien `mailto:`.  
Pour personnaliser l'adresse et l'objet du mail :

```html
<a href="mailto:contact@podcastzone.com?subject=Je%20souhaite%20en%20savoir%20plus%20sur%20votre%20plateforme" class="contact-button">
  ✉️ Nous contacter
</a>
