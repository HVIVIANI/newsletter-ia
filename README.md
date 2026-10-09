# Veille IA — page d'inscription

Page d'inscription à **Veille IA**, une newsletter quotidienne sur l'actualité de l'intelligence artificielle, conçue et opérée par [Hugo Viviani](https://www.linkedin.com/in/hugo-viviani-a4b298228/).

**La page : https://hviviani.github.io/newsletter-ia/**

## Ce que fait la newsletter

Chaque matin, un script lit 26 sources (blogs des laboratoires, presse, newsletters, communautés), soit environ 340 articles, et n'en garde que les signaux forts : 5 en moyenne. Pour chaque sujet : un titre, deux ou trois phrases qui ne disent que ce qui figure dans les articles, un statut (officiel, confirmé, déclaration, accusation, rumeur) et les liens vers les sources.

## Comment fonctionne l'inscription

| Pièce | Rôle | Où |
|---|---|---|
| Cette page | Le formulaire | GitHub Pages (ce dépôt) |
| Le script | Enregistre l'inscription, envoie l'e-mail de confirmation, gère le désabonnement | Google Apps Script |
| La liste des abonnés | Nom, prénom, société, adresse, statut | Un Google Sheet privé |

1. Le formulaire envoie les informations au script.
2. Le script envoie un e-mail de confirmation. Rien d'autre n'est envoyé tant que la personne n'a pas cliqué.
3. Chaque newsletter contient un lien de désabonnement personnel.

Aucune donnée personnelle n'est stockée dans ce dépôt : il ne contient que la page.

## Limites connues

- L'envoi passe par un compte Gmail gratuit, limité à 100 e-mails par jour. Au-delà d'environ 90 abonnés, les nouveaux inscrits passent en liste d'attente.
- Les trois chiffres affichés en haut de la page sont des moyennes relevées en octobre 2026. Le temps gagné est une estimation : 340 titres à parcourir, environ 5 secondes chacun.

## Fichiers

- `index.html` : la page, sans dépendance externe.
- `apercu.png` : l'image affichée quand le lien est partagé.
