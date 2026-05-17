# 📋 Réponses du Quiz — Quishing

> Revenez ici après avoir répondu aux questions dans le [README](../README.md).

---

## Question 1 ✅ Bonne réponse : **B**

> *Vous recevez un email de votre banque avec un QR code vous demandant de "vérifier votre compte".*

**Réponse B — Appeler sa banque directement via le numéro officiel** ✔️

**Explication :**
Une banque légitime ne vous demandera **jamais** de scanner un QR code pour "vérifier" ou "sécuriser" votre compte. Cette demande est un signal d'alarme classique du quishing.

- ❌ **A** : Même si l'email semble venir de votre banque, l'adresse peut être usurpée (*spoofing*). Ne scannez jamais sans vérifier.
- ✅ **B** : Appeler via le **numéro au dos de votre carte** ou sur le site officiel (tapé manuellement) est la seule méthode sûre.
- ❌ **C** : Répondre à l'email contacte l'attaquant, pas votre banque.
- ❌ **D** : Même sans rien entrer, accéder au site peut déclencher des malwares ou confirmer que votre adresse est active.

---

## Question 2 ✅ Bonne réponse : **B**

> *Dans un parking, vous remarquez que le QR code de l'horodateur a l'air d'être un sticker collé par-dessus.*

**Réponse B — Chercher un autre horodateur ou payer en espèces** ✔️

**Explication :**
Un sticker QR code par-dessus un autre est un **signe quasi-certain d'une attaque quishing**. Des dizaines de cas ont été documentés en France depuis 2022.

- ❌ **A** : Ne jamais ignorer ce signal d'alerte visuel.
- ✅ **B** : La prudence est de mise. Un autre horodateur non modifié ou le paiement en espèces est la solution la plus sûre.
- ⚠️ **C** : Arracher le sticker peut être une bonne idée pour signaler l'anomalie aux autorités, mais pas avant d'avoir contacté la mairie ou la police pour le signaler.
- ❌ **D** : L'application de scan ne change rien : c'est l'URL de destination qui est malveillante, pas le QR code lui-même.

**💡 Conseil bonus** : Signalez toujours ce type d'anomalie à la mairie ou à la police locale.

---

## Question 3 ✅ Bonne réponse : **B**

> *Pourquoi les attaquants utilisent-ils des QR codes dans les emails plutôt que des liens cliquables ?*

**Réponse B — Ça contourne les filtres anti-spam** ✔️

**Explication :**
C'est précisément **pour ça que le quishing est si efficace**. Les systèmes de sécurité email (filtres anti-spam, antivirus, sandboxes) analysent le texte et les liens dans les emails. Mais un QR code, c'est **une image** — et les machines ne "lisent" pas les images aussi facilement.

| Technique | Détecté par les filtres ? |
|-----------|--------------------------|
| Lien texte malveillant | ✅ Souvent détecté |
| QR code dans une image | ❌ Rarement détecté |

- ❌ **A** : Créer un QR code n'est pas plus simple qu'un lien.
- ✅ **B** : Bonne réponse — contournement des systèmes de détection automatique.
- ❌ **C** : Les études montrent l'inverse : les gens font davantage confiance aux liens texte connus qu'aux QR codes.
- ❌ **D** : L'esthétique n'est pas la motivation des cybercriminels.

---

## Question 4 ✅ Bonne réponse : **B**

> *Quelle est la meilleure façon de vérifier si un site est légitime après avoir scanné un QR code ?*

**Réponse B — Vérifier l'URL complète avant de charger la page** ✔️

**Explication :**
La plupart des smartphones affichent une **prévisualisation de l'URL** avant d'ouvrir le lien après un scan. C'est le moment crucial pour vérifier.

**Ce qu'il faut regarder :**
```
✅ https://impots.gouv.fr/accueil
❌ https://impots-gouv.fr.verification.com/accueil
❌ https://impots.gouv.fr.fake-site.top/
❌ http://impots.gouv.fr/accueil  (pas de HTTPS !)
```

- ❌ **A** : Les faux sites sont souvent des copies quasi-parfaites de l'original. L'apparence visuelle ne suffit pas.
- ✅ **B** : L'URL est la vérification la plus fiable.
- ❌ **C** : Entrer de fausses informations peut quand même confirmer à l'attaquant que votre compte existe (si la page "valide" les données).
- ⚠️ **D** : Le cadenas HTTPS signifie que la connexion est chiffrée, **pas** que le site est légitime. Un site frauduleux peut très bien avoir un certificat SSL valide.

---

## 📊 Votre score

| Score | Niveau | Message |
|-------|--------|---------|
| 4/4 | 🏆 Expert | Vous êtes bien sensibilisé(e) ! Partagez ces connaissances autour de vous. |
| 3/4 | ✅ Bon niveau | Bonne base, relisez les explications des questions ratées. |
| 2/4 | ⚠️ À améliorer | Relisez le README et repassez le quiz dans quelques jours. |
| 0-1/4 | 🚨 Attention | Prenez le temps de lire l'ensemble du dépôt — c'est important ! |

---

*← Retour au [README principal](../README.md)*
