# CogiSearch

<p align="center"><img alt="Logo CogiSearch" title="CogiSearch" src="https://raw.githubusercontent.com/cogilabs/CogiSearch/main/cogiSearch.svg"></p>

<p align="center">
    <img alt="HTML5" title="Conçu avec HTML5" src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white"/>
    <img alt="CSS3" title="Stylisé avec CSS3" src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white"/>
    <img alt="JavaScript" title="Propulsé par JavaScript" src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"/>
    <img alt="Site Statique" title="Aucun traitement côté serveur" src="https://img.shields.io/badge/Site-Statique-4285F4?style=for-the-badge"/>
</p>

<p align="center">
    <a href="https://search.cogilabs.eu" target="_blank"><img alt="Visiter CogiSearch" title="Essayez maintenant !" src="https://img.shields.io/badge/Visiter-CogiSearch-brightgreen?style=for-the-badge"/></a>
    <a href="#ajouter-à-votre-navigateur"><img alt="Ajouter au Navigateur" title="Instructions d'installation" src="https://img.shields.io/badge/Ajouter_à-Votre_Navigateur-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white"/></a>
</p>

[→ In English](/README.md)  

## Table des matières

- [Introduction](#introduction)
- [Fonctionnalités](#fonctionnalités)
- [Utilisation](#utilisation)
- [Auto-hébergement](#auto-hébergement)
- [Personnalisation](#personnalisation)
- [Licence](#licence)

## Introduction

CogiSearch est un routeur de recherche qui vous permet d'utiliser le concept de "*bangs*" de <a href="https://duckduckgo.com/">DuckDuckGo</a> pour rechercher rapidement sur différents moteurs. Contrairement à DuckDuckGo, CogiSearch vous permet de définir votre propre moteur de recherche par défaut et offre une expérience plus rapide et personnalisable.

Un "bang" est un raccourci spécial qui redirige votre recherche vers un moteur de recherche spécifique. Par exemple, taper `!g chats` recherchera "chats" sur Google.

## Fonctionnalités

- 🔍 **Routage de recherche rapide** : Redirige instantanément vos requêtes vers vos moteurs de recherche préférés
- 🔄 **Sélection du moteur par défaut** : Définissez n'importe quel moteur de recherche comme moteur par défaut (y compris via une URL personnalisée)
- 🛠️ **Bangs personnalisés** : Accès à tous les bangs de DuckDuckGo plus des ajouts spécifiques
- 🌐 **URL personnalisée pour moteur** : Définissez votre propre moteur de recherche en utilisant `%s` comme placeholder
- 🌓 **Thème clair/sombre** : Basculez entre les modes clair et sombre
- 📋 **Intégration facile** : Ajoutez CogiSearch à n'importe quel navigateur avec une simple URL
- 💾 **Aucun suivi** : Vos recherches ne sont ni stockées ni suivies

## Utilisation

### Recherche de base

1. Saisissez votre requête dans la barre de recherche
2. Ajoutez un bang n'importe où dans votre requête pour utiliser un moteur spécifique (ex. `!g` pour Google)
3. Si aucun bang n'est spécifié, votre moteur de recherche par défaut sera utilisé

### Bangs populaires

<table>
    <thead>
        <tr>
            <th>Bang</th>
            <th>Moteur de recherche</th>
            <th>Exemple</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><code>!g</code></td>
            <td>Google</td>
            <td><code>!g meilleur langage de programmation</code></td>
        </tr>
        <tr>
            <td><code>!b</code></td>
            <td>Bing</td>
            <td><code>!b idées de vacances</code></td>
        </tr>
        <tr>
            <td><code>!y</code></td>
            <td>Yahoo</td>
            <td><code>!y prévisions météo</code></td>
        </tr>
        <tr>
            <td><code>!qw</code></td>
            <td>Qwant</td>
            <td><code>!qw outils de confidentialité</code></td>
        </tr>
        <tr>
            <td><code>!brave</code></td>
            <td>Brave Search</td>
            <td><code>!brave messagerie sécurisée</code></td>
        </tr>
        <tr>
            <td><code>!yt</code></td>
            <td>YouTube</td>
            <td><code>!yt tutoriels cuisine</code></td>
        </tr>
        <tr>
            <td><code>!w</code></td>
            <td>Wikipédia</td>
            <td><code>!w les Backrooms</code></td>
        </tr>
    </tbody>
</table>

### Définir votre moteur de recherche par défaut

1. Visitez la page d'accueil de CogiSearch
2. Faites défiler jusqu'à la section Paramètres
3. Choisissez entre :
   - Sélectionner un moteur populaire
   - Saisir un bang personnalisé
   - Fournir une URL de moteur personnalisée (`https://exemple.com/search?q=%s`)
4. Votre choix sera sauvegardé automatiquement pour vos recherches futures

> **Note** : Lors de l'utilisation d'une URL personnalisée, `%s` sera remplacé dynamiquement par votre requête.

### Ajouter à votre navigateur

Pour ajouter CogiSearch comme moteur de recherche dans votre navigateur :

1. Copiez cette URL : `https://search.cogilabs.eu/?q=%s`
2. Dans les paramètres de moteur de recherche de votre navigateur :
  - **Chrome** : Paramètres → Moteur de recherche → Gérer les moteurs de recherche → Ajouter
  - **Firefox** : Paramètres → Recherche → Ajouter un moteur de recherche → Autre
  - **Edge** : Paramètres → Confidentialité, recherche et services → Barre d'adresse et recherche → Gérer les moteurs de recherche → Ajouter
3. Nommez-le "CogiSearch" et collez l'URL
4. Définissez-le comme moteur de recherche par défaut (optionnel)

## Auto-hébergement

CogiSearch est un site web statique qui peut être hébergé sur n'importe quel serveur :

1. Clonez le dépôt : `git clone https://github.com/cogilabs/cogisearch.git`
2. Uploadez les fichiers sur votre serveur
3. Accédez à votre site via votre domaine

Aucun traitement côté serveur n'est nécessaire : tout fonctionne en JavaScript côté client.

## Personnalisation

### Ajouter des bangs personnalisés

Vous pouvez maintenant ajouter vos propres bangs personnalisés directement depuis l'interface utilisateur :

1. Faites défiler jusqu'à la section **Bangs utilisateur** sur la page principale
2. Entrez le nom de votre bang dans le premier champ
3. Entrez l'URL dans le second champ, en utilisant `%s` comme placeholder pour la requête de recherche
4. Cliquez sur le bouton "Ajouter Bang"

Vos bangs personnalisés seront stockés dans le stockage local de votre navigateur et immédiatement disponibles pour vos recherches. Vous pouvez en ajouter autant que nécessaire et les supprimer à tout moment. Ces bangs personnalisés continuent d'exister entre les sessions de navigation sur le même appareil.

Exemple :
- Nom du bang : `reddit`
- URL : `https://www.reddit.com/search?q=%s`

Cela créera un bang `!reddit` qui recherchera directement sur Reddit.  
  
Les bangs créés de cette façon écraseront tous les bangs existants avec le même déclencheur.

### Définir une URL de moteur personnalisée

Vous pouvez également définir une URL personnalisée sans créer de bang.

Exemple :

- Entrez `https://exemple.com/recherche?q=%s` dans le champ URL personnalisé
- `%s` sera automatiquement remplacé par votre requête de recherche

Cela permet d'utiliser **n'importe quel moteur de recherche** prenant en charge les requêtes directes !

> Exemple d'URL personnalisée : `https://github.com/search?q=%s` permettra de rechercher directement sur GitHub.

## Licence

CogiSearch est sous licence MIT. Voir [LICENSE](/LICENSE) pour plus d'informations.

---

<p align="center">Propulsé par <a href="https://Cogilabs.eu/">Cogilabs.eu</a></p>
