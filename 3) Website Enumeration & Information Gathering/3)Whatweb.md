# 🕵️ WhatWeb et son utilisation

🌍 **WhatWeb** est un outil de reconnaissance qui permet d'identifier les technologies utilisées sur les sites web. Il reconnaît les technologies web telles que les systèmes de gestion de contenu (CMS), les plateformes de blogging, les frameworks statistiques et analytiques, les systèmes de JavaScript, et bien plus encore.

## 🛠️ Utilisation de WhatWeb :

### 🌐 Identification des technologies :
- WhatWeb peut identifier et rapporter les types de technologies utilisées sur un site web.
- Cela peut inclure des informations sur les versions de CMS, les plugins utilisés, les technologies de serveur web, etc.

### 🔒 Sécurité et audit :
- Dans un contexte de sécurité, WhatWeb peut être utilisé pour identifier les technologies obsolètes ou vulnérables utilisées sur un site web.
- Crucial pour l'évaluation de la sécurité d'un site.

### 🔎 Reconnaissance :
- Les professionnels de la cybersécurité utilisent WhatWeb pour recueillir des informations sur les cibles potentielles.
- Aide à préparer des tests de pénétration ou des audits de sécurité.

## 💻 Lignes de commande utilisées pendant le cours

### `whatweb --help` :
- 📚 Cette commande affiche l'aide et les options disponibles pour l'outil WhatWeb.
- Utile pour comprendre toutes les fonctionnalités et les paramètres que WhatWeb peut prendre.

### `man whatweb` :
- 📘 Ouvre le manuel de WhatWeb, fournissant des informations détaillées sur son utilisation, ses options et son fonctionnement.

### `whatweb --aggression 3 -v IP` :
- 🎯 Lance WhatWeb sur l'adresse IP spécifiée avec un niveau d'agression de 3 (agressif) et en mode verbeux (-v).

### `whatweb --aggression 3 -v IP/24` :
- 📡 Cette commande lance WhatWeb sur une plage d'adresses IP (subnet) avec le même niveau d'agression et en mode verbeux.

### `whatweb --aggression 3 -v IP/24 --no-errors` :
- 🚫 Exécute la même commande que ci-dessus mais avec l'option --no-errors, empêchant l'affichage des erreurs.
