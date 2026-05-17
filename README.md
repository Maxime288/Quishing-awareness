# 🔍 Sensibilisation au Quishing

> **Quishing** = **QR** + **Phishing** — Une cyberattaque qui utilise des QR codes malveillants pour voler vos données.

![Badge](https://img.shields.io/badge/Cybersécurité-Sensibilisation-red?style=for-the-badge)
![Badge](https://img.shields.io/badge/Niveau-Débutant%20à%20Intermédiaire-orange?style=for-the-badge)
![Badge](https://img.shields.io/badge/Langue-Français-blue?style=for-the-badge)

---

## 📋 Table des matières

1. [C'est quoi le Quishing ?](#-cest-quoi-le-quishing-)
2. [Comment ça fonctionne ?](#-comment-ça-fonctionne-)
3. [Exemples d'attaques réelles](#-exemples-dattaques-réelles)
4. [Comment se protéger ?](#-comment-se-protéger-)
5. [Quiz de sensibilisation](#-quiz-de-sensibilisation)
6. [Ressources](#-ressources)
7. [Contribuer](#-contribuer)

---

## 🎯 C'est quoi le Quishing ?

Le **quishing** (contraction de *QR code* et *phishing*) est une technique d'hameçonnage qui utilise des **QR codes frauduleux** pour rediriger les victimes vers des sites malveillants.

### Pourquoi c'est dangereux ?

- ✅ Les QR codes semblent **légitimes** et inoffensifs
- ✅ Les antivirus et filtres email **ne les détectent pas facilement**
- ✅ Sur mobile, l'URL de destination est **difficile à vérifier avant d'ouvrir**
- ✅ Les gens font **confiance aux QR codes** dans les lieux publics, restaurants, gares...

---

## ⚙️ Comment ça fonctionne ?

```
[Attaquant crée un QR code malveillant]
           │
           ▼
[QR code placé : email, affiche, colis, parking...]
           │
           ▼
[Victime scanne le QR code avec son téléphone]
           │
           ▼
[Redirection vers un faux site (copie de banque, Microsoft, impôts...)]
           │
           ▼
[La victime entre ses identifiants / données bancaires]
           │
           ▼
[L'attaquant récupère les données → Vol d'identité / argent]
```

### Les 3 phases d'une attaque quishing

| Phase | Description | Exemple |
|-------|-------------|---------|
| **1. Création** | L'attaquant génère un QR code pointant vers un site frauduleux | Faux site `impots-gouv-fr.com` |
| **2. Distribution** | Le QR code est diffusé (email, affiches, stickers...) | Email prétendant venir de votre banque |
| **3. Exploitation** | La victime scanne et entre ses données | Vol de mot de passe ou données bancaires |

---

## 🕵️ Exemples d'attaques réelles

### 1. Faux horodateurs de parking 🅿️
Des stickers avec de faux QR codes sont collés par-dessus les vrais sur les horodateurs. La victime croit payer son stationnement mais donne ses coordonnées bancaires à l'attaquant.

> 💡 **Cas réel** : Ce type d'arnaque a été signalé dans plusieurs grandes villes françaises (Paris, Lyon, Bordeaux) depuis 2022.

### 2. Quishing par email 📧
Un email prétendant venir de Microsoft, votre banque ou les impôts contient un QR code au lieu d'un lien cliquable. Pourquoi ? Parce que les filtres anti-spam analysent les liens texte mais **pas les QR codes dans les images**.

```
Objet : ⚠️ Votre compte sera suspendu dans 24h - Action requise
De : support@microsoft-security.com

Bonjour,

Une activité suspecte a été détectée sur votre compte.
Veuillez scanner ce QR code pour sécuriser votre compte :

[IMAGE QR CODE MALVEILLANT]

Cordialement,
L'équipe Microsoft
```

**🚩 Signaux d'alerte dans cet email :**
- Urgence artificielle ("24h")
- Expéditeur douteux (domaine non officiel)
- QR code au lieu d'un lien direct
- Pression psychologique

### 3. Restaurants et menus frauduleux 🍽️
Des QR codes faux sont placés sur les tables de restaurants à la place ou par-dessus les originaux, redirigeant vers de faux menus qui demandent des informations personnelles.

### 4. Livraison de colis 📦
Faux SMS ou emails de livraison (La Poste, Chronopost...) avec un QR code pour "reprogrammer votre livraison", menant à un site frauduleux qui vole vos données de carte bancaire.

---

## 🛡️ Comment se protéger ?

### ✅ Bonnes pratiques

1. **Vérifiez l'URL AVANT d'ouvrir**
   - La plupart des appareils affichent l'URL avant redirection
   - Cherchez des fautes d'orthographe : `impots-gouv.fr` ≠ `impots.gouv.fr`
   - Méfiez-vous des domaines en `.xyz`, `.top`, `.click`

2. **Inspectez le QR code physiquement**
   - Un sticker par-dessus un autre QR code = signe d'alerte
   - Si le QR code semble collé ou décalé, ne le scannez pas

3. **N'entrez jamais vos données après avoir scanné un QR code reçu par email**
   - Allez directement sur le site officiel en tapant l'URL vous-même

4. **Utilisez une application de scan avec prévisualisation**
   - Certaines apps affichent l'URL complète avant de l'ouvrir

5. **Activez l'authentification à deux facteurs (2FA)**
   - Même si vos identifiants sont volés, le pirate ne pourra pas accéder à votre compte sans le second facteur

### ❌ Ce qu'il ne faut JAMAIS faire

- ❌ Scanner un QR code reçu par email de manière inattendue
- ❌ Entrer vos données bancaires ou mots de passe après un scan
- ❌ Ignorer les avertissements de votre navigateur sur un site non sécurisé
- ❌ Faire confiance à un QR code uniquement parce qu'il est dans un lieu officiel
- ❌ Cliquer sur "Ignorer l'avertissement" si votre téléphone vous alerte

---

## 🧠 Quiz de sensibilisation

Testez vos connaissances ! Les réponses sont dans le fichier [`answers.md`](answers.md).

**Question 1** : Vous recevez un email de votre banque avec un QR code vous demandant de "vérifier votre compte". Que faites-vous ?
- A) Je scanne le QR code car c'est ma banque
- B) J'appelle ma banque directement via le numéro officiel
- C) Je clique sur "Répondre" pour demander confirmation
- D) Je scanne mais n'entre rien

**Question 2** : Dans un parking, vous remarquez que le QR code de l'horodateur a l'air d'être un sticker collé par-dessus. Vous...
- A) Scannez quand même, c'est probablement normal
- B) Cherchez un autre horodateur ou payez en espèces
- C) Arrachez le sticker pour voir en dessous
- D) Scannez mais avec une autre application

**Question 3** : Pourquoi les attaquants utilisent-ils des QR codes dans les emails plutôt que des liens cliquables ?
- A) C'est plus facile à créer
- B) Ça contourne les filtres anti-spam qui analysent les liens texte
- C) Les gens cliquent plus facilement sur les QR codes
- D) C'est plus esthétique

**Question 4** : Quelle est la meilleure façon de vérifier si un site est légitime après avoir scanné un QR code ?
- A) Regarder si le site ressemble à l'original
- B) Vérifier l'URL complète avant de charger la page
- C) Tester en entrant de fausses informations
- D) Regarder s'il y a un cadenas dans le navigateur

---

## 📚 Ressources

### Sites officiels français
- 🇫🇷 [cybermalveillance.gouv.fr](https://www.cybermalveillance.gouv.fr) — Assistance aux victimes de cyberattaques
- 🇫🇷 [ANSSI](https://www.ssi.gouv.fr) — Agence nationale de la sécurité des systèmes d'information
- 🇫🇷 [Signal Spam](https://www.signal-spam.fr) — Signalement de spams et tentatives de phishing

### Signaler une attaque
- **Phishing** : [phishing-initiative.fr](https://www.phishing-initiative.fr)
- **Fraude bancaire** : Contactez votre banque immédiatement
- **Cybermalveillance** : [cybermalveillance.gouv.fr](https://www.cybermalveillance.gouv.fr)
- **Police** : [pre-plainte-en-ligne.gouv.fr](https://www.pre-plainte-en-ligne.gouv.fr)

### Pour aller plus loin
- 📄 [Fiche technique : Les arnaques aux QR codes - CNIL](https://www.cnil.fr)
- 🎓 [MOOC SecNumacadémie - ANSSI](https://secnumacademie.gouv.fr) (gratuit)
- 📺 Documentaire : "Hackers, la menace fantôme" - Arte

---

## 📂 Structure du dépôt

```
quishing-sensibilisation/
│
├── README.md                    ← Vous êtes ici
├── quiz/
│   ├── questions.md             ← Quiz de sensibilisation
│   └── answers.md               ← Réponses commentées
├── exemples/
│   ├── email-quishing.png       ← Exemple d'email frauduleux annoté
│   ├── parking-quishing.png     ← Exemple de QR code parking frauduleux
│   └── sms-quishing.png         ← Exemple de SMS frauduleux
├── affiches/
│   ├── affiche-sensibilisation.pdf  ← Affiche à imprimer
│   └── infographie-quishing.pdf     ← Infographie explicative
└── presentation/
    └── slides-quishing.pdf      ← Support de présentation
```

---

## 🤝 Contribuer

Les contributions sont les bienvenues ! Si vous souhaitez améliorer ce dépôt :

1. Forkez le projet
2. Créez une branche (`git checkout -b feature/nouvelle-ressource`)
3. Committez vos modifications (`git commit -m 'Ajout : exemple d'attaque quishing en entreprise'`)
4. Pushez (`git push origin feature/nouvelle-ressource`)
5. Ouvrez une Pull Request

---

## ⚠️ Projet à but éducatif uniquement

Ce projet a été créé exclusivement dans un objectif de sensibilisation à la cybersécurité, d’éducation et de formation défensive.

L’auteur n’encourage ni ne soutient aucune activité illégale liée au phishing, au quishing ou au vol de données.

Toutes les démonstrations, reproductions de pages et scénarios présentés dans ce dépôt sont réalisés dans un environnement de test contrôlé à des fins pédagogiques uniquement.

---

## 👤 Auteur

**Maxime FAU** — [@Maxime288](https://github.com/Maxime288)
Lycée Jules Fil

> 💬 *"La meilleure défense contre le quishing, c'est la connaissance."*

---

*⭐ Si ce projet vous a été utile, n'hésitez pas à lui mettre une étoile !*
