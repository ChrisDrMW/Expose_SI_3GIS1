# Fonctions de hachage
## Introduction
## I. Defs
Une fonction de hachage est donc une fonction mathématique qui prend comme argument une chaine de bits de longueur arbitraire finie (le message) et restitue en sortie une chaîne de longueur fixée : l'empreinte ou haché ou encore condensat.
- **fonction simple :** celle qui calcule directement et simplement le hash
- **fonction cryptographique** : celle qui possède des propriétés de sécurité
## II. motivations
### 1. fonctions simples
- table de hachage
- CRC
### 2. fonctions cryptographiques
- vérifier l'intégrité des données
- pour l'authentification des messages
- dans la signature électronique
- protection de mots de pass
- Dérivation de clé dans la crypto symétrique
- Protocoles d'engagement : engagement sans divulgation d'informations
- Génération de nombres pseudo-aléatoires
- techno blockchain
## III. Fonctions de hachage cryptographiques
### 1. Propriétés classiques
- résistance aux collisions
- résistance au calcul d'antécédent
- résistance au calcul de second antécédent
### 2. Construction des fonctions cryptographiques
Un paradigme : primitive opérant sur un domaine de taille fixe + extenseur de domaine.
    \---> Premieres propositions : Rabin 78, Merkle 79
    \---> fonctions itératives [LM92] : algo de compression + extenseur
Autres approches : 
- hachage par paquet
- Randomize-then-Combine Paradigm
- Arbres de Merkle (P2P networks)

fonctions de compression (**discours**):
	- basées sur un schema de chiffrement par bloc (famille MD-SHA)
	- basées sur un pb réputé difficile

extenseurs : 
- Merkle-Damgard (+ utilisé en pratique(années ???))
- éponge cryptographique : fn de hachage proche d'un oracle aléatoire
- Wide-Pipe & Double-Pipe (resistance multi-collisions dans Merkle-D)
- HAIFA (renforce la sécu des constructions itératives % attaques génériques)
- EMD, ROX, plus théoriques avec objectif : preservation d'un grand nb de pptés de la fn de compression. -- > preuve : fondée sur une famille de fonctions de compression

## IV. Présentation des différentes fonctions de hachage cryptographiques (niveaux de secu)
??? Presentation historique : Davies-Meyer, Matias-Meyer-Oseas, MDC-2, MDC-4, MD2, MD4, MD5, SHA-0, SHA-1, SHA-2, SHA-3(?)
	- breve description ou principe de fonctionnement ?
	- utilisation actuelle ?
## V. Cryptanalyse des fonctions cryptographiques ?
## Conclusion

***
# Signatures numériques
## Introduction
 - def
 - importance (dans la sécurité de l'information)
## Principes de base de la crypto asymétrique
## Infrastructures de Gestion des clés

- Certificats numériques
- Autorités de certification (CA)
- Format X.509
- Chaînes de confiance
## Fonctionnement d'une signature numérique
- etape 1 : hachage du message
- etape 2  : chiffrement du hash avec la clé privée
- etape 3 : verification avec la clé publique
- Démonstration schématique
## Techniques ou algorithmes de signatures numériques
- RSA
- DSA
- ECDSA
- EdDSA
- Schémas post-quantiques 
	- Crystalls-Dilithium
	- Falcon
	- SPHINCS+

## Limites et menaces
- compromission de clé privée
- Faibles algorithmes (RSA trop court, SHA-1, DSA mal utilisé)
- faux certificats / attaques de l'infrastructure PKI
- Importance de la révocation (CRL, OCSP)
## Types de signatures numériques
- signature simple : on signe un message avec sa clé privée.
- signature avancée : signature associée à l’identité du signataire via un certificat
- signature qualifiée : repose sur un certificat émis par une autorité reconnue
- signature détachée / attachée : integrée ou non dans le fichier
- signature en anneau
- signature aveugle
- signature agrégées
## Applications en sciences de l'information
- Signature de documents administratifs
- authentification dans les systèmes d'information
- signature de logiciels et mises à jour
- Transactions électroniques (banque, e-commerce)
- Horodatage et archivage numérique

## Conclusion
