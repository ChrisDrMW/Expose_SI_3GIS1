# Fonctions de hachage
## Introduction
## I. Définition
## II. motivations
## III. Fonctions de hachage cryptographiques
### 1. Propriétés classiques (sens unique, faible et forte resistance aux collisions)
### 2. Construction des fonctions de hachage cryptographiques
Une approche naturelle pour construire les fonctions de hachage consiste à définir une fonction qui **opère sur un domaine de taille fixe** puis d'étendre ce domaine grâce à un **extenseur de domaine**. Dans ce cadre nous présenterons 2 extenseurs et verrons comment sont construits 2/3 algorithmes de hachage.

**extenseurs**
Nous allons présenter deux extenseurs :
- Merkle-Damgard
- éponge cryptographique
**Fonctions de hachage :**
-  MD5
- SHA-2

## V. Cryptanalyse des fonctions cryptographiques (2/3 points)
## Conclusion

***
# Signatures numériques
## Introduction
 - def
 - importance (dans la sécurité de l'information)
## Motivations
## Principes de base de la crypto asymétrique + PKI (CA, certificat numérique, format X.509, chaine de confiance)

## Techniques de signatures numériques
Nous allons traiter 3 exemples classique et 1 exemple post-quantique
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
## Conclusion
