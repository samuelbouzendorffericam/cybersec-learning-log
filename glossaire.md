# Glossaire de cybersécurité

Notions de base, expliquées simplement.

## Principes

- **Triade CID (confidentialité, intégrité, disponibilité)** : les trois propriétés à protéger. Confidentialité : seuls les ayants droit accèdent à l'information. Intégrité : elle n'est pas modifiée sans autorisation. Disponibilité : elle est accessible quand on en a besoin.
- **Authentification / autorisation** : l'authentification vérifie *qui* vous êtes, l'autorisation détermine *ce que* vous avez le droit de faire.
- **Principe du moindre privilège** : chaque compte ou programme ne reçoit que les droits strictement nécessaires.
- **Défense en profondeur** : empiler plusieurs couches de protection pour qu'une seule faille ne suffise pas.
- **MFA (authentification multifacteur)** : combiner au moins deux preuves d'identité (mot de passe + code temporaire, clé physique...).

## Cryptographie

- **Hachage** : transformation à sens unique d'une donnée en une empreinte de taille fixe (SHA-256). Sert à vérifier l'intégrité et à stocker les mots de passe.
- **Sel (salt)** : valeur aléatoire ajoutée à un mot de passe avant de le hacher, pour que deux mots de passe identiques n'aient pas la même empreinte.
- **Chiffrement symétrique** : la même clé chiffre et déchiffre (AES). Rapide, mais il faut partager la clé.
- **Chiffrement asymétrique** : une clé publique chiffre, une clé privée déchiffre (RSA). Sert à échanger des clés et à signer.
- **Certificat TLS** : document qui lie une clé publique à l'identité d'un site, à la base du cadenas HTTPS.

## Menaces et vulnérabilités

- **Vulnérabilité** : faiblesse dans un système. **Exploit** : moyen concret d'en profiter.
- **CVE** : identifiant public d'une vulnérabilité connue (ex. CVE-2021-44228). **CVSS** : note de gravité de 0 à 10.
- **Faille 0-day** : vulnérabilité exploitée avant que l'éditeur ne dispose d'un correctif.
- **Phishing (hameçonnage)** : message qui imite une source de confiance pour voler des identifiants ou faire cliquer.
- **Ingénierie sociale** : manipuler une personne plutôt qu'une machine pour obtenir un accès ou une information.
- **Brute force** : essayer systématiquement des mots de passe jusqu'à trouver le bon.
- **Injection SQL** : saisie malveillante interprétée comme du code par la base de données ; se prévient avec des requêtes paramétrées.
- **XSS (Cross-Site Scripting)** : injection de script dans une page web vue par d'autres utilisateurs.
- **OWASP Top 10** : liste des dix catégories de risques les plus courants pour les applications web.
- **Ransomware** : logiciel qui chiffre les données et demande une rançon.

## Défense et organisation

- **Pare-feu** : filtre le trafic réseau selon des règles.
- **IDS / IPS** : système qui détecte (IDS) ou bloque (IPS) les activités suspectes.
- **SIEM** : outil qui centralise et corrèle les journaux pour repérer des incidents.
- **VPN** : tunnel chiffré entre un appareil et un réseau.
- **Pentest (test d'intrusion)** : attaque simulée, autorisée et encadrée, pour trouver des failles avant les vrais attaquants.
- **Red team / Blue team** : la red team joue les attaquants, la blue team défend et détecte.
- **CTF (Capture The Flag)** : compétition où l'on résout des épreuves de sécurité pour récupérer des « drapeaux ».
