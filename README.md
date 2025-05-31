# 🛡️ Guide Progressif de la Sécurité Informatique

Un parcours pédagogique pour comprendre la cybersécurité, avec définitions, exemples, schémas, et des questions/exercices de type examen corrigés.  
Inclut des QCM, cas concrets, outils, et exercices théoriques.

---

## 1️⃣ Fondamentaux de la Cybersécurité

### 🔒 Qu’est-ce que la cybersécurité ?
La cybersécurité regroupe les techniques, outils et bonnes pratiques pour protéger systèmes, réseaux et données contre les attaques, le vol ou la destruction.

---

### 🎯 Objectifs de Sécurité

| Objectif          | Définition                                                      | Exemple concret                          |
|-------------------|-----------------------------------------------------------------|------------------------------------------|
| Confidentialité   | Accès réservé aux personnes autorisées                          | Mot de passe chiffré                     |
| Intégrité         | Données non modifiées sans autorisation                         | Bulletin modifiable uniquement par admin |
| Disponibilité     | Services et données accessibles quand nécessaire                | Site disponible 24/7                     |
| Authenticité      | Vérifier l’identité de l’utilisateur ou machine                 | Connexion par identifiants               |
| Non-répudiation   | Impossible de nier une action réalisée                          | Signature numérique d’un contrat         |

---

## 2️⃣ Vulnérabilités, Menaces, Impact

| Vulnérabilité                   | Menace      | Impact                        |
|----------------------------------|-------------|-------------------------------|
| Interface compliquée             | Erreur humaine | Base de données corrompue   |
| Mots de passe en clair           | Pirate      | Usurpation de compte          |
| Logiciel non mis à jour          | Malware     | Interception des communications|

---

## 3️⃣ Phases d’une Attaque

1. **Reconnaissance** : collecte d’infos (outil : Nmap)
2. **Scan** : recherche active de failles
3. **Exploitation** : utilisation d’une faille pour entrer
4. **Maintien, Effacement** : rester discret, pivoter

---

## 4️⃣ Principales Attaques

- **DoS/DDoS** : saturer un service (Smurf Attack)
- **Sniffing** : espionner le trafic réseau
- **ARP Spoofing** : détourner le trafic local
- **Brute Force** : tester beaucoup de mots de passe
- **Phishing** : usurper une identité pour voler des infos

---

## 5️⃣ Outils de Cybersécurité

| Outil           | Définition & Utilité                              | Exemple d’utilisation                |
|-----------------|---------------------------------------------------|--------------------------------------|
| Pare-feu (Firewall) | Filtre le trafic selon des règles             | Bloquer le port 23                   |
| IDS/IPS         | Détection (IDS) et blocage (IPS) d’attaques       | Détecter un scan de port             |
| Nmap            | Scanner de ports et services                      | Lister les ports ouverts d’un serveur |
| Wireshark       | Analyseur de paquets réseau                       | Voir les paquets sur un réseau Wi-Fi  |
| OpenVAS/Nessus  | Scanner de vulnérabilités                         | Détecter des failles sur un serveur   |
| Antivirus       | Détection/suppression de logiciels malveillants   | Supprimer un virus                   |

---

## 6️⃣ Défenses, Chiffrement et Authentification

- **Chiffrement symétrique** : même clé pour chiffrer et déchiffrer (ex : AES)
- **Chiffrement asymétrique** : paire clé publique/privée (ex : RSA, ECC)
- **Signature numérique** : preuve d’origine & d’intégrité (ex : signer un PDF)
- **Certificat électronique** : garantit l’identité d’un serveur (ex : HTTPS)

---

## 7️⃣ VPN et DMZ

- **VPN** : tunnel sécurisé sur Internet (mode tunnel : site à site, transport : client à site)
- **DMZ** : zone tampon pour isoler les serveurs exposés

---

## 8️⃣ Exercices/QCM Niveau Examen + Réponses

---

### QCM Outils & Concepts

**1. Lequel des outils suivants permet d’analyser les paquets réseau ?**  
A) Nmap  
B) Wireshark  
C) Nessus  
D) OpenVAS  
**Réponse :** B) Wireshark

---

**2. Le scanner de vulnérabilité le plus utilisé en entreprise est :**  
A) Wireshark  
B) Nmap  
C) Nessus  
D) Fail2Ban  
**Réponse :** C) Nessus

---

**3. À quoi sert un pare-feu ?**  
A) Chiffrer les données  
B) Filtrer le trafic réseau  
C) Détecter les virus  
D) Stocker les logs  
**Réponse :** B) Filtrer le trafic réseau

---

**4. Quel outil est principalement utilisé pour scanner les ports d’une machine ?**  
A) Nessus  
B) Nmap  
C) IDS  
D) VPN  
**Réponse :** B) Nmap

---

**5. Quel est le rôle d’un IDS ?**  
A) Analyser les paquets  
B) Détecter les intrusions  
C) Chiffrer les communications  
D) Bloquer les accès  
**Réponse :** B) Détecter les intrusions

---

### Exercices Théoriques Corrigés

---

**1. Explique la différence entre un IDS et un IPS.**  
- IDS (Intrusion Detection System) détecte les attaques et alerte, mais ne bloque pas.
- IPS (Intrusion Prevention System) détecte ET bloque automatiquement les attaques.

---

**2. Donne deux exemples d’attaques et les outils pour les détecter.**  
- Sniffing (Wireshark)  
- Scan de ports (Nmap, détectable par IDS)

---

**3. Qu’est-ce qu’une signature numérique ? Donne un cas d’usage.**  
- C’est une empreinte du message chiffrée avec la clé privée de l’expéditeur, servant à prouver l’origine et l’intégrité.  
- Exemple : signer un contrat PDF pour qu’il soit légalement opposable.

---

**4. Quelle est la différence entre chiffrement symétrique et asymétrique ?**  
- Symétrique : Une seule clé secrète partagée.  
- Asymétrique : Paire clé publique/clé privée (clé publique diffuse, privée secrète).

---

**5. Pourquoi utiliser un certificat électronique pour HTTPS ?**  
- Pour garantir l’identité du serveur et chiffrer la connexion grâce à une autorité de certification reconnue.

---

**6. Qu’est-ce qu’une DMZ et à quoi sert-elle ?**  
- Zone intermédiaire pour placer les serveurs accessibles depuis Internet, afin de protéger le réseau interne en cas de compromission.

---

**7. Cite deux méthodes pour détecter une attaque sur le réseau.**  
- Détection par signature : comparaison avec des motifs connus (IDS/IPS)
- Détection comportementale : détection d’anomalies dans le trafic

---

**8. Explique le principe d’un VPN site-à-site.**  
- C’est un tunnel chiffré reliant deux réseaux distants, permettant aux machines de chaque site de communiquer comme si elles étaient sur le même réseau local.

---

**9. Donne un exemple de situation où la non-répudiation est essentielle.**  
- Lors de la signature d’un contrat en ligne ou d’une transaction bancaire électronique.

---

**10. Pourquoi faut-il éviter de transmettre les mots de passe en clair sur un réseau ?**  
- Parce qu’ils peuvent être interceptés via du sniffing, ce qui permettrait l’usurpation de compte.

---

# 🎓 Conseils pour réviser

- Associe toujours chaque outil à son usage principal
- Pour chaque concept, trouve un exemple réel
- Retiens les différences clés (ex : IDS ≠ IPS ; chiffrement ≠ hachage)
- Entraîne-toi avec des QCM et des mini-cas pratiques

---

**La cybersécurité, c’est comprendre les risques, maîtriser les outils, et rester attentif aux évolutions !**
