# ARIA — Politique de confidentialité

> **Avis sur la version qui prévaut.** La présente version française est la
> traduction officielle de la politique de confidentialité d'ARIA. **Pour les
> consommateurs résidant au Québec, c'est la version française qui prévaut** en cas
> de divergence avec la version anglaise, conformément à la *Charte de la langue
> française* (RLRQ, c. C-11). Cette traduction devrait être révisée par un juriste
> avant sa diffusion publique.

**Dernière mise à jour : 25 juillet 2026**
**Date d'entrée en vigueur : 25 juillet 2026**

La présente politique de confidentialité explique comment ARIA (« ARIA »,
« l'application », « nous », « notre », « nos ») traite vos renseignements. ARIA est
un assistant de finances personnelles, d'agenda et de tâches pour iPhone. Elle
repose sur une promesse simple : **vos données vivent sur votre appareil, et nous
ne les vendons jamais.**

ARIA est fournie par **Boris Alexander Legkow Orias**, un développeur individuel
exerçant comme travailleur autonome au **Québec, Canada** (« le développeur »). Le
développeur est l'entreprise responsable de vos renseignements personnels au sens
de la **Loi 25 du Québec** (la Loi sur la protection des renseignements personnels
dans le secteur privé), de la loi fédérale **LPRPDE** et — pour les utilisateurs de
ces régions — du **RGPD de l'UE/du Royaume-Uni** (à titre de responsable du
traitement) et de la **CCPA/CPRA de Californie**.

- **Personne responsable de la protection des renseignements personnels
  (responsable de la protection des renseignements personnels) :**
  Boris Alexander Legkow Orias
- **Coordonnées :** legkow@me.com
- **Adresse postale :** 1 rue Boucher, Port-Cartier, QC G5B 2T9, Canada
- **Site Web :** https://legkow.github.io/aria-legal

Les résidents du Québec sont visés par la **Loi 25**; les autres utilisateurs
canadiens et tout renseignement personnel qui traverse une frontière provinciale ou
nationale sont visés par la **LPRPDE**. Lorsque plus d'une loi pourrait
s'appliquer, nous appliquons la **norme la plus élevée**.

> **Résumé en langage clair.** Presque tout ce que vous saisissez dans ARIA reste
> sur votre iPhone. Si vous activez la synchronisation, vos données sont chiffrées
> sur votre appareil au moyen d'une clé qui demeure dans votre trousseau iCloud —
> accessible par vos autres appareils, mais jamais par nous — de sorte que même
> nous ne pouvons pas les lire. Certaines fonctions sont optionnelles et ne
> s'exécutent que lorsque vous les activez : relier une banque (Plaid) ou importer
> votre agenda (Google/Apple). Les fonctions d'IA s'exécutent sur votre appareil —
> au moyen des modèles d'Apple, ou d'un modèle ouvert facultatif que vous pouvez
> choisir de télécharger. Nous ne vous suivons pas d'une application ou d'un site Web à
> l'autre, nous n'exécutons aucun SDK publicitaire et nous ne vendons pas vos
> données. Ce résumé n'est fourni que par commodité; c'est le texte complet ci-dessous
> qui fait foi.

---

## 1. Personnes visées par la présente politique

La présente politique s'applique à toute personne qui utilise l'application iOS
ARIA. Elle vise les données que vous saisissez, les données qu'ARIA lit à partir
des services que vous choisissez de relier, ainsi que les données limitées
nécessaires au fonctionnement de votre compte et de votre abonnement.

ARIA est destinée à un **public général d'adultes**. Elle **n'est pas destinée aux
enfants**, et nous ne recueillons pas sciemment leurs données : ni celles d'un
mineur de moins de **14 ans** au Québec (l'âge auquel la Loi 25 rattache le
consentement parental), de moins de **16 ans** dans l'UE/au Royaume-Uni, ni de
moins de **13 ans** aux États-Unis. Voir la section 11. *(Il s'agit des âges
auxquels des lois particulières sur la protection des renseignements personnels
exigent le consentement parental pour la collecte de données — ces âges sont
plus restreints que l'âge minimal général pour utiliser ARIA prévu aux
Conditions d'utilisation, soit **16 ans, ou 18 ans lorsque requis** — voir
l'article 2 des Conditions d'utilisation, et ne le modifient pas.)*

---

## 2. Les données qu'ARIA traite, et où elles résident

ARIA fonctionne **d'abord en local** (local-first). Sauf si une ligne ci-dessous
indique que des données sont « transmises », elles sont stockées uniquement sur
votre appareil (dans le magasin SwiftData d'Apple et le trousseau iOS) et ne sont
jamais envoyées à nous ni à qui que ce soit d'autre.

| Données | Exemples | Comment ARIA les obtient | Où elles vont |
|---|---|---|---|
| **Dossiers financiers** | Noms et soldes de comptes, transactions (commerçant, montant, date, catégorie), factures, budgets, objectifs, montants de filet de sécurité, abonnements | Vous les saisissez; vous importez un fichier CSV; ou vous reliez une banque au moyen de Plaid | Sur l'appareil. Si la synchronisation est activée, incluses dans la sauvegarde **chiffrée de bout en bout**. |
| **Données bancaires via Plaid** | Soldes de comptes, historique des transactions, masque du compte (4 derniers chiffres) | Uniquement si vous reliez une banque dans Plaid Link | Récupérées côté serveur par notre infrastructure dorsale et livrées à votre appareil. Voir la section 5. **En lecture seule — ARIA ne déplace jamais d'argent.** |
| **Événements d'agenda** | Titres d'événements, dates, heures | Agenda Apple (EventKit) ou Google Agenda, en lecture seule, uniquement si vous les reliez; ou vous créez des événements dans ARIA | Sur l'appareil. Si la synchronisation est activée, incluses dans la sauvegarde chiffrée. |
| **Tâches et projets** | Titres de tâches, dates d'échéance, étiquettes, projets, étapes | Vous les saisissez, ou vous les ajoutez par la voix au moyen de Siri | Sur l'appareil. Si la synchronisation est activée, incluses dans la sauvegarde chiffrée. |
| **Votre nom** | Prénom | Vous le fournissez facultativement à la connexion | Sur l'appareil; rattaché à votre compte si vous utilisez la synchronisation infonuagique. |
| **Identifiant de compte** | Identifiant utilisateur Apple (de Se connecter avec Apple) | Se connecter avec Apple | Envoyé à notre infrastructure dorsale pour créer et authentifier votre compte. |
| **Adresse courriel** | — | **Non demandée.** Se connecter avec Apple peut transmettre votre adresse (ou une adresse de relais privé d'Apple), mais ARIA ne demande à Apple que votre prénom : aucune adresse ne nous est donc jamais transmise. | Nulle part. Votre dossier de compte ne contient aucune adresse courriel. (Si vous nous écrivez pour du soutien, nous détenons évidemment ce message — voir la section 14.) |
| **Photos de reçus** | Une photo d'un reçu | Uniquement si vous numérisez un reçu | Traitée **sur l'appareil** pour lire le commerçant, le montant et la date, puis **supprimée**. L'image n'est jamais stockée ni transmise. |
| **Saisie vocale** | Ce que vous dites à ARIA — vous pouvez toucher le micro pour lancer puis arrêter l'écoute, ou le maintenir enfoncé et le relâcher quand vous avez terminé | Microphone + reconnaissance vocale sur l'appareil | Transcrite **sur votre appareil** (`requiresOnDeviceRecognition`), utilisée pour répondre, puis supprimée. Ni stockée, ni transmise. |
| **Face ID / données biométriques** | Résultat de correspondance biométrique | Verrouillage facultatif de l'application | Géré entièrement par iOS (LocalAuthentication). ARIA ne voit ni ne stocke jamais de données biométriques. |
| **Diagnostics (facultatif)** | Événements d'utilisation grossiers et non identifiants (p. ex. « fonction ouverte ») | Uniquement si vous activez « Statistiques d'utilisation » (désactivé par défaut) | Voir la section 6. Ne contient aucun nom, courriel ni montant. |
| **État d'abonnement/d'achat** | Si vous disposez d'ARIA+ | Achat sur l'App Store via RevenueCat | Voir la section 5. |
| **Réglages de l'appareil** | Apparence, devise, langue, personnalité d'ARIA, préférences de notification | Vous les réglez | Sur l'appareil (`UserDefaults` / `@AppStorage`). |

Nous ne recueillons **pas** : votre adresse courriel (nous ne la demandons jamais à
Apple — voir le tableau ci-dessus), vos identifiants de connexion bancaire (ceux-ci
vont directement à Plaid, jamais à ARIA), votre localisation précise, vos contacts,
vos identifiants publicitaires, ni aucun contenu de courriel — ARIA ne demande jamais
d'accès à Gmail ni à aucun autre service de courriel.

---

## 3. Pourquoi nous traitons vos données, et nos bases juridiques (RGPD)

Lorsque le RGPD/le RGPD du Royaume-Uni s'applique, nous nous appuyons sur les bases
juridiques suivantes (art. 6) :

| Finalité | Base juridique |
|---|---|
| Faire fonctionner les fonctions essentielles de l'application sur votre appareil (suivi de l'argent, des factures, des tâches, de l'agenda) | **Exécution d'un contrat** (art. 6(1)(b)) — vous nous avez demandé de fournir ARIA |
| Authentifier votre compte et synchroniser votre sauvegarde chiffrée | **Exécution d'un contrat** (art. 6(1)(b)) |
| Relier une banque (Plaid) ou importer un agenda (Google/Apple) | **Consentement** (art. 6(1)(a)) — ces fonctions sont désactivées jusqu'à ce que vous les activiez, et vous pouvez retirer votre consentement à tout moment |
| Traiter le verrouillage biométrique de l'application | **Consentement** — et géré par iOS, jamais par nous |
| Diagnostics facultatifs | **Consentement** (désactivé par défaut) |
| Gérer votre abonnement ARIA+ | **Exécution d'un contrat** (art. 6(1)(b)) |
| Maintenir la sécurité du service, prévenir les abus et respecter les obligations légales | **Intérêts légitimes** (art. 6(1)(f)) et **obligation légale** (art. 6(1)(c)) |

Vous pouvez retirer votre consentement à tout moment en déconnectant l'intégration
concernée dans les Réglages ou en désactivant la fonction. Le retrait du
consentement n'a pas d'incidence sur le traitement déjà effectué.

**Consentement, et consentement exprès pour les renseignements sensibles.** Nous
demandons votre consentement au moyen de choix clairs, précis et distincts — chaque
intégration optionnelle (Plaid, Google Agenda) et la synchronisation
infonuagique sont désactivées jusqu'à ce que vous les activiez. Comme vos
**renseignements financiers sont sensibles**, nous demandons votre consentement
**exprès** avant que vous reliiez une banque ou que nous traitions vos données
financières, et nous les utilisons uniquement aux fins que vous avez activées.

---

## 4. Intelligence sur l'appareil et IA

L'« intelligence » d'ARIA — le score de vie (Life Score), les suggestions
proactives, la lecture des reçus, la détection des abonnements, les signalements
d'anomalies et l'assistant vocal — s'exécute **sur votre appareil** au moyen des
**modèles de fondation (Foundation Models)** d'Apple intégrés à l'appareil, avec une
logique déterministe sur l'appareil pour le calcul des scores et la détection des
tendances.

- **Rien n'est envoyé hors de votre appareil pour l'IA.** Dans cette version, chaque
  requête d'IA reçoit sa réponse sur votre appareil. ARIA n'a pas recours à **Apple
  Private Cloud Compute** (l'environnement serveur d'Apple respectueux de la vie
  privée) — ce chemin n'est pas activé dans l'application publiée. Si une version
  future l'active, nous le dirons d'abord ici.
- **Un second modèle facultatif, lui aussi sur l'appareil.** Activer **Réglages →
  ARIA → Sur l'appareil uniquement** restreint le modèle d'Apple strictement à votre
  appareil et télécharge un petit modèle ouvert (Qwen3-1.7B, 4 bits, licence
  Apache-2.0, environ 1 Go, par Wi-Fi) depuis la plateforme de modèles Hugging Face.
  Sur les iPhone dépourvus d'Apple Intelligence, c'est ce modèle téléchargé qui
  formule les réponses d'ARIA — et, comme celui d'Apple, il s'exécute entièrement sur
  votre appareil. Le téléchargement ne récupère **que les poids du modèle** : aucune
  donnée vous concernant n'est transmise à Hugging Face ni à qui que ce soit d'autre.
  Le modèle n'est téléchargé que si vous le demandez — soit en activant ce réglage, soit
  en touchant Télécharger dans le lecteur de relevés PDF, sous Finances › Importer. Si
  vous ne faites ni l'un ni l'autre, rien n'est téléchargé, ARIA se rabattant alors sur
  des formulations gabarit simples.
- **Nous n'envoyons vos données à aucun fournisseur d'IA tiers** (pas d'OpenAI, pas
  d'Anthropic, pas de Google AI). Il n'y a aucune IA infonuagique facturée au jeton
  dans ARIA.
- Les résultats de l'IA sont informatifs et peuvent être erronés. ARIA fait
  ressortir des tendances dans vos propres données; elle **ne fournit pas** de
  conseils financiers, de placement, fiscaux ou juridiques. Voir les Conditions
  d'utilisation.
- **Traitement automatisé et profilage.** ARIA établit des constats à partir d'un
  profil de vos propres données (le score de vie, le montant « disponible à
  dépenser », les signalements d'anomalies, les suggestions). Ceux-ci sont
  **informatifs** et ne constituent **pas** des décisions prises uniquement par une
  machine produisant des effets juridiques ou des effets significatifs comparables —
  c'est vous qui décidez quoi faire. Si nous devions un jour introduire une telle
  décision automatisée, nous vous en informerions, nous expliquerions les principaux
  facteurs utilisés, nous vous permettrions de faire corriger les données sous-jacentes
  et de demander qu'une personne procède à un examen.

---

## 5. Services tiers avec lesquels nous travaillons

ARIA fait appel à un petit nombre de fournisseurs. Nous ne communiquons **que ce
dont chaque fonction a besoin**, et uniquement lorsque vous utilisez cette fonction.
Chaque fournisseur est un responsable du traitement ou un sous-traitant indépendant
soumis à sa propre politique de confidentialité.

### Plaid — connexion bancaire (optionnel)
Si vous reliez une banque, vous le faites au moyen de **Plaid Link**. Vous saisissez
vos identifiants bancaires **directement auprès de Plaid** — ARIA ne les voit ni ne
les stocke jamais. Plaid renvoie des données de compte et de transactions, que notre
infrastructure dorsale récupère pour votre compte et livre à votre appareil. Le
jeton d'accès Plaid est conservé **uniquement côté serveur**; votre appareil ne
détient qu'un identifiant d'élément opaque. La connexion est en **lecture seule**;
ARIA ne peut pas déplacer d'argent, effectuer de paiements ou amorcer de virements,
et ne le fait pas. Votre utilisation de Plaid est aussi régie par la **politique de
confidentialité des utilisateurs finaux** de Plaid :
https://plaid.com/legal/#end-user-privacy-policy. Vous pouvez déconnecter une banque
à tout moment dans les Réglages, ce qui dissocie l'élément.

### Google — Agenda (optionnel)
Si vous reliez Google Agenda, ARIA demande un accès en **lecture seule**
(`calendar.readonly`) au moyen de Google OAuth. Les jetons OAuth sont stockés dans
le trousseau de votre appareil. ARIA ne demande **aucun** accès à Gmail — aucune
portée liée aux courriels n'est jamais demandée, et aucun contenu de courriel
n'est lu.

> **Divulgation d'utilisation limitée (Limited Use).** L'utilisation et le transfert
> par ARIA des renseignements reçus des API Google sont conformes à la
> [politique de Google relative aux données utilisateur des services API](https://developers.google.com/terms/api-services-user-data-policy),
> y compris ses exigences d'**utilisation limitée** (Limited Use). Plus précisément :
> nous accédons aux données de Google Agenda uniquement pour fournir et améliorer les
> fonctions internes que vous demandez (afficher vos événements); nous traitons ces
> données **sur votre appareil**; nous **ne** les transférons **pas** à des tiers,
> sauf dans la mesure nécessaire pour fournir ces fonctions, pour des raisons de
> sécurité ou pour nous conformer à la loi; nous **ne** les utilisons **pas** à des
> fins publicitaires; et nous **ne** permettons **pas** à des humains de les lire,
> sauf avec votre consentement, pour des raisons de sécurité ou si la loi l'exige.

### Apple — comptes, agenda, achats, intelligence
ARIA utilise des cadriciels Apple : **Se connecter avec Apple** (création de
compte), **EventKit** (Agenda Apple), **StoreKit** (achats), **Speech**
(transcription sur l'appareil), **LocalAuthentication** (Face ID), **ActivityKit**
(activités en direct) et **Foundation Models** (intelligence sur l'appareil). Le
traitement de ces données par Apple est régi par la politique de
confidentialité d'Apple (https://www.apple.com/legal/privacy/).

### RevenueCat — gestion des abonnements
Les abonnements ARIA+ sont traités au moyen de l'App Store d'Apple et gérés à l'aide
de **RevenueCat**, qui valide votre reçu de l'App Store et indique à l'application si
votre abonnement est actif. RevenueCat reçoit un identifiant d'utilisateur
d'application pseudonyme ainsi que des données d'achat et de reçu; il ne reçoit pas
vos dossiers financiers, votre agenda ni vos courriels. Voir la politique de
confidentialité de RevenueCat : https://www.revenuecat.com/privacy.

### Cloudflare — notre infrastructure dorsale et la synchronisation chiffrée
Notre infrastructure dorsale de compte, de synchronisation et de Plaid fonctionne
sur **Cloudflare Workers**, un réseau informatique périphérique mondial — notre
déploiement n'est pas fixé à un seul pays, de sorte que les requêtes peuvent être
traitées dans n'importe quelle installation de Cloudflare dans le monde, y
compris aux États-Unis. Elle stocke votre sauvegarde de
synchronisation **chiffrée de bout en bout** (que nous ne pouvons pas déchiffrer),
votre dossier de compte et — uniquement côté serveur — votre jeton d'accès Plaid.
Cloudflare agit comme notre sous-traitant d'hébergement.

Nous tenons à jour une liste des sous-traitants, disponible sur demande à
legkow@me.com.

---

## 6. Statistiques et suivi

- ARIA ne comporte **aucun SDK publicitaire** et n'effectue **aucun suivi d'une
  application ou d'un site à l'autre**. Nous n'utilisons pas l'identifiant
  publicitaire (IDFA) et ne présentons pas d'invite de transparence du suivi des
  applications (App Tracking Transparency), parce que nous ne vous suivons pas. Notre
  manifeste de confidentialité Apple déclare **« Données non utilisées pour vous
  suivre ».**
- **Les statistiques d'utilisation sont à activation facultative et désactivées par
  défaut.** Si vous les activez dans les Réglages, ARIA n'enregistre que des
  événements grossiers et **non identifiants** (par exemple, quelle fonction a été
  ouverte) — jamais votre nom, votre courriel ni un montant d'argent. Désactiver le
  réglage efface ce qui a été stocké. Les statistiques d'utilisation sont de
  **première partie et demeurent sur votre appareil** — aucun fournisseur d'analyse
  tiers n'est utilisé (l'intégration PostHog envisagée a été retirée). **MetricKit**
  d'Apple fournit des diagnostics de panne et de performance sur l'appareil, et l'App
  Store peut nous transmettre des statistiques d'utilisation **agrégées et anonymes**
  au moyen de son propre App Analytics (uniquement si vous avez activé le réglage
  Apple « Partager avec les développeurs d'apps » sur votre appareil). Si une version
  future transmet ces diagnostics à nos serveurs, ils demeureront exempts
  d'identifiants personnels et nous mettrons d'abord à jour la présente politique.

---

## 7. Comment nous communiquons les données

Nous **ne vendons pas** vos renseignements personnels, et nous ne les
**« communiquons » pas à des fins de publicité comportementale intercontextuelle**,
au sens donné à ces termes par la California Consumer Privacy Act (CCPA/CPRA). Nous
n'avons ni vendu ni communiqué de renseignements personnels au cours des 12 derniers
mois.

Nous ne communiquons des données que :
- aux fournisseurs mentionnés à la section 5, strictement pour faire fonctionner les
  fonctions que vous utilisez;
- si la loi, une procédure judiciaire ou une demande gouvernementale valide l'exige;
- pour protéger les droits, la sécurité ou la sûreté des utilisateurs ou du public;
  ou
- dans le cadre d'un transfert d'entreprise (p. ex. si l'application est acquise),
  auquel cas nous vous en aviserons et la présente politique continuera de
  s'appliquer à vos données.

---

## 8. Conservation des données

- **Les données sur l'appareil** demeurent jusqu'à ce que vous les supprimiez, que
  vous supprimiez l'application ou que vous supprimiez votre compte.
- **La sauvegarde de synchronisation chiffrée** est conservée tant que votre compte
  est actif et supprimée lorsque vous supprimez votre compte (voir la section 9).
- **Les images de reçus** ne sont jamais stockées — elles sont traitées une seule
  fois puis supprimées.
- **La saisie vocale** est éphémère et supprimée après avoir servi à vous répondre.
- **Les diagnostics facultatifs** sont plafonnés à une petite mémoire tampon locale
  et effacés lorsque vous désactivez les statistiques.
- **Les dossiers de compte et de Plaid** sur notre infrastructure dorsale sont
  supprimés lorsque vous supprimez votre compte, sous réserve de toute brève
  conservation requise pour des raisons de sécurité ou légales. Le reçu d'essai
  pseudonyme décrit ci-dessous constitue la seule exception.
- **Les horodatages anticontournement** — quelques dates dans le trousseau de votre
  appareil (le début de votre essai gratuit de 3 jours, la dernière exécution de
  l'application, la dernière synchronisation bancaire) — sont conservés pour la durée
  de vie de l'appareil, afin que l'essai et les limites d'actualisation bancaire ne
  puissent pas être réinitialisés en supprimant puis en réinstallant l'application.
  Ce sont des dates et rien d'autre : aucun nom, compte, montant ni coordonnée, et
  elles ne quittent jamais votre appareil. Pour un compte vérifié, notre serveur
  conserve aussi un reçu pseudonyme permanent contenant uniquement l'horodatage du
  premier début d'essai et celui de la création du reçu. Sa clé est dérivée par un
  hachage à sens unique de votre identifiant de compte stable; il ne contient aucun
  identifiant brut, nom, courriel, renseignement financier ni jeton Plaid. Il sert
  uniquement à empêcher la même identité vérifiée de relancer l'essai ou son quota
  de banques après une suppression de compte, une réinstallation ou un changement
  d'appareil. Voir la section 9.

---

## 9. Vos droits et vos choix

**Commandes dans l'application (accessibles à tous) :**
- **Exporter mes données** — téléchargez une copie complète de vos dossiers au format
  JSON (Réglages → Données). L'exportation est toujours accessible et n'est jamais
  restreinte par votre abonnement.
- **Supprimer le compte** — une seule action, partout. Elle efface votre compte et
  votre sauvegarde de synchronisation chiffrée sur notre infrastructure dorsale;
  révoque chaque banque reliée auprès de Plaid ainsi que toute autorisation Google
  Agenda connectée; détruit votre clé de chiffrement de synchronisation et votre
  identifiant de session; supprime chaque dossier sur votre appareil, y compris tout
  fichier d'exportation écrit par ARIA et ses caches de travail; et annule les
  notifications en attente. Cette action est irréversible. La suppression du compte
  est toujours accessible et n'est jamais restreinte par votre abonnement. Deux
  éléments limités subsistent délibérément, et aucun ne contient votre contenu ARIA
  ni vos données financières :
  - **Les horodatages anticontournement** — quelques dates dans le trousseau de votre
    appareil (le début de votre essai gratuit de 3 jours, la dernière exécution de
    l'application, la dernière synchronisation bancaire). Elles n'existent que pour
    empêcher la réinitialisation de l'essai gratuit et des limites d'actualisation
    bancaire par une suppression suivie d'une réinstallation, ou par un recul de
    l'horloge de l'appareil. Elles ne contiennent aucun nom, compte, courriel ni
    donnée financière, sont marquées « cet appareil seulement » et ne quittent jamais
    votre téléphone ni n'atteignent nos serveurs. Pour un compte vérifié, un reçu
    pseudonyme distinct subsiste aussi sur le serveur : les horodatages du premier
    début d'essai et de création du reçu, sous une clé dérivée par SHA-256. Il ne
    contient aucun identifiant de compte brut ni autre contenu de compte et sert
    uniquement à empêcher la réinitialisation de l'essai par suppression-recréation,
    réinstallation ou changement d'appareil.
  - **Un abonnement, le cas échéant.** ARIA+ est facturé par Apple : supprimer votre
    compte ARIA ne l'annule donc pas. Annulez dans **Réglages → votre compte Apple →
    Abonnements**.
- **Déconnecter les intégrations** — dissociez Plaid ou Google Agenda à tout
  moment.
- **Désactiver la synchronisation / utiliser hors ligne** — gardez toutes les données
  uniquement sur l'appareil.
- **Désactiver les diagnostics** — efface les événements stockés.

**Droits dans l'UE/au Royaume-Uni (RGPD).** Vous pouvez demander l'accès, la
rectification, l'effacement, la limitation, la portabilité et l'opposition, et vous
pouvez retirer votre consentement à tout moment. Plusieurs de ces droits sont
accessibles directement dans l'application (exportation/suppression). Pour toute
autre demande, écrivez à legkow@me.com. Nous répondons dans un délai de
**30 jours** (prolongeable de 60 jours pour les demandes complexes). Vous avez aussi
le droit de déposer une plainte auprès de votre autorité de contrôle. ARIA est
offerte sur l'App Store au **Canada et aux États-Unis** et n'est ni commercialisée ni
destinée à l'UE ou au Royaume-Uni; lorsque ces droits vous sont néanmoins
applicables, vous pouvez les exercer en écrivant au responsable de la protection des
renseignements personnels, à l'adresse indiquée au début de la présente politique.

**Droits en Californie (CCPA/CPRA).** Vous pouvez demander de connaître, de
supprimer et de corriger vos renseignements personnels, et de limiter l'utilisation
des renseignements personnels sensibles. Nous ne vendons ni ne communiquons vos
renseignements personnels et nous n'exerçons aucune discrimination à votre égard
parce que vous exercez vos droits. Nous accusons réception des demandes dans un délai
de **10 jours ouvrables** et y répondons dans un délai de **45 jours** (prolongeable
de 45 jours). Soumettez vos demandes à legkow@me.com.

**Droits au Canada — Québec (Loi 25) et LPRPDE.** Vous pouvez :
- **accéder** aux renseignements personnels que nous détenons à votre sujet et les
  **rectifier**;
- recevoir les renseignements que vous nous avez fournis dans un **format structuré
  et couramment utilisé** (nous fournissons le format **JSON**) — la **portabilité
  des données** — ou les faire transmettre à un autre organisme que vous autorisez
  (cela vise les renseignements que vous avez fournis, et non les valeurs qu'ARIA
  infère, comme le score de vie);
- **retirer votre consentement** à tout moment, et nous demander de cesser la
  diffusion de vos renseignements ou de les désindexer lorsque la loi le permet;
- être informé de tout traitement automatisé, comme il est décrit à la section 4.

Nous répondons dans un délai de **30 jours**. Si nous refusons une demande, nous en
expliquons les motifs et vous indiquons comment en demander la révision. Vous pouvez
également porter plainte auprès d'un organisme de réglementation : au **Québec**,
auprès de la **Commission d'accès à l'information (CAI)** — cai.gouv.qc.ca; ailleurs
au **Canada**, auprès du **Commissariat à la protection de la vie privée du Canada
(CPVP)** — priv.gc.ca, 1-800-282-1376. Nous rendons la présente politique
accessible au public et en fournirons une copie sur demande.

Nous vérifions les demandes au moyen de mesures raisonnables et proportionnées aux
données en cause. Comme nous ne détenons aucune adresse courriel vous concernant
(voir la section 2), la preuve habituelle est le contrôle du compte Apple avec lequel
vous vous êtes connecté : vous connecter à ARIA et utiliser les commandes
d'exportation ou de suppression dans l'application en fait la démonstration à soi
seul. Pour une demande envoyée par courriel, nous pouvons vous demander des
précisions que seul le titulaire du compte connaîtrait — et nous en demandons le
moins possible, jamais un identifiant bancaire ni une pièce d'identité
gouvernementale.

---

## 10. Sécurité

- **Chiffrement de bout en bout.** Votre sauvegarde de synchronisation est chiffrée
  sur votre appareil au moyen de **AES-256-GCM** à l'aide d'une clé de 256 bits.
  Cette clé est conservée dans votre **trousseau iCloud**, qu'Apple chiffre
  elle-même de bout en bout, de sorte qu'elle puisse atteindre en toute sécurité
  vos autres appareils Apple sans jamais transiter par — ni être lisible par —
  nos serveurs. Nous ne recevons jamais la clé et ne pouvons pas lire vos
  données synchronisées.
- **En transit**, tout le trafic réseau utilise HTTPS/TLS.
- **Au repos sur l'appareil**, votre justificatif de session est stocké
  uniquement sur l'appareil dans le trousseau iOS (`ThisDeviceOnly`, jamais
  synchronisé); les identifiants bancaires ne sont jamais traités par ARIA.
- Aucune méthode de stockage ou de transmission n'est sûre à 100 %. Si un **incident
  de confidentialité** (atteinte à la protection des données) survient, nous en
  évaluons le risque et réagissons comme la loi l'exige :
  - **Québec (Loi 25) :** lorsque l'incident présente un **risque qu'un préjudice
    sérieux soit causé**, nous en avisons avec diligence la **Commission d'accès à
    l'information** et les personnes concernées, et nous tenons un registre des
    incidents.
  - **Canada (LPRPDE) :** lorsqu'une atteinte crée un **risque réel de préjudice
    grave**, nous la signalons au **Commissariat à la protection de la vie privée du
    Canada** et vous en avisons dès que possible.
  - **UE/Royaume-Uni (RGPD) :** nous avisons l'autorité de contrôle compétente dans
    un délai de **72 heures** lorsque cela est requis, et les utilisateurs concernés
    sans retard injustifié lorsque le risque est élevé.

---

## 11. Enfants

ARIA n'est pas destinée aux enfants. Nous ne recueillons pas sciemment de
renseignements personnels auprès d'un mineur de moins de **14 ans** au Québec (où la
Loi 25 rattache le consentement à un parent ou à un tuteur), de moins de **16 ans**
dans l'UE/au Royaume-Uni, ni de moins de **13 ans** aux États-Unis (COPPA). Si vous
croyez qu'un enfant nous a fourni des données, communiquez avec
legkow@me.com et nous les supprimerons.

---

## 12. Communication hors du Québec / du Canada, et transferts internationaux

Notre infrastructure dorsale et nos fournisseurs de services (Cloudflare,
RevenueCat, Plaid, Google) sont des entreprises établies aux États-Unis, et le
réseau de Cloudflare traite des données dans des installations partout dans le
monde (non fixées à un seul pays) — de sorte que certains de vos renseignements
(votre dossier de compte; si vous reliez une banque, un jeton d'accès côté
serveur; et votre sauvegarde de synchronisation chiffrée de bout en bout) sont
**communiqués hors du Québec et du Canada**.

- Pour les résidents du **Québec**, avant de faire appel à un fournisseur situé
  hors du Québec, nous procédons à l'évaluation des facteurs relatifs à la vie
  privée que la Loi 25 exige, et nous exigeons que nos fournisseurs soient liés
  par des modalités de traitement des données proportionnées à la sensibilité
  des renseignements qu'ils traitent (nous sommes en train de formaliser des
  ententes signées avec chaque fournisseur et mettrons à jour la présente
  section une fois ce processus terminé); notre position repose entre-temps sur
  le **chiffrement de bout en bout** (aucun hébergeur, aux États-Unis ou
  ailleurs, ne peut lire votre contenu synchronisé) et sur la minimisation des
  données.
- Pour les autres utilisateurs **canadiens**, nous demeurons responsables en vertu de
  la LPRPDE et exigeons par contrat que nos fournisseurs protègent vos données selon
  une norme comparable.
- Pour les utilisateurs de l'**UE/du Royaume-Uni**, les transferts reposent sur des
  garanties appropriées, notamment les **clauses contractuelles types de l'UE** et
  l'**addenda relatif au transfert international de données du Royaume-Uni**.

Votre **contenu synchronisé est chiffré de bout en bout et illisible en transit
comme au repos** par nous et par notre fournisseur d'hébergement.

---

## 13. Modifications de la présente politique

Nous pouvons mettre à jour la présente politique à mesure que l'application évolue ou
que la loi change. Nous publierons la version mise à jour avec une nouvelle date de
« Dernière mise à jour » et, en cas de modifications importantes, nous en
donnerons un avis dans l'application. La poursuite de l'utilisation après une mise à
jour signifie que vous acceptez la politique révisée.

---

## 14. Coordonnées

Questions, demandes ou plaintes :
**legkow@me.com**
Boris Alexander Legkow Orias · 1 rue Boucher, Port-Cartier, QC G5B 2T9, Canada

---

*ARIA est un outil informatif. Elle n'est ni une banque, ni un transmetteur de
fonds, ni un conseiller financier, et elle ne déplace pas d'argent. Voir les
Conditions d'utilisation pour plus de détails.*
