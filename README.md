# CogiSearch

<p align="center"><img alt="CogiSearch Logo" title="CogiSearch" src="https://raw.githubusercontent.com/cogilabs/CogiSearch/main/cogiSearch.svg"></p>

<p align="center">
    <img alt="HTML5" title="Built with HTML5" src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white"/>
    <img alt="CSS3" title="Styled with CSS3" src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white"/>
    <img alt="JavaScript" title="Powered by JavaScript" src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"/>
    <img alt="Static Website" title="No server-side processing" src="https://img.shields.io/badge/Static-Website-4285F4?style=for-the-badge"/>
</p>

<p align="center">
    <a href="https://search.cogilabs.eu" target="_blank"><img alt="Visit CogiSearch" title="Try it now!" src="https://img.shields.io/badge/Visit-CogiSearch-brightgreen?style=for-the-badge"/></a>
    <a href="#adding-to-your-browser"><img alt="Add to Browser" title="Setup Instructions" src="https://img.shields.io/badge/Add_to-Your_Browser-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white"/></a>
</p>

[→ En Français](/localizedReadme/README-fr.md)  

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Usage](#usage)
- [Self-Hosting](#self-hosting)
- [Customizing](#customizing)
- [License](#license)

## Introduction

CogiSearch is a search router that allows you to use the idea of "*bangs*" from <a href="https://duckduckgo.com/">DuckDuckGo</a> to quickly search across different engines. Unlike DuckDuckGo, CogiSearch lets you set your own default search engine and provides a faster, more customizable experience.

A "bang" is a special shortcut that redirects your search to a specific search engine. For example, typing `!g cats` will search for "cats" on Google.

## Features

- 🔍 **Fast Search Routing**: Instantly redirects your queries to your preferred search engines
- 🔄 **Default Engine Selection**: Set any search engine as your default
- 🌓 **Light/Dark Theme**: Toggle between light and dark mode for comfortable browsing
- 📋 **Easy Integration**: Add CogiSearch to any browser with a simple URL
- 🛠️ **Custom Bangs**: Access to all DuckDuckGo bangs plus custom additions
- 💾 **No Tracking**: Your searches aren't stored or tracked

## Usage

### Basic Searching

1. Enter your search query in the search box
2. Add a bang at the beginning of your query to use a specific search engine (e.g., `!g` for Google)
3. If no bang is specified, your default search engine will be used

### Popular Bangs

<table>
    <thead>
        <tr>
            <th>Bang</th>
            <th>Search Engine</th>
            <th>Example</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><code>!g</code></td>
            <td>Google</td>
            <td><code>!g best programming language</code></td>
        </tr>
        <tr>
            <td><code>!b</code></td>
            <td>Bing</td>
            <td><code>!b vacation ideas</code></td>
        </tr>
        <tr>
            <td><code>!y</code></td>
            <td>Yahoo</td>
            <td><code>!y weather forecast</code></td>
        </tr>
        <tr>
            <td><code>!qw</code></td>
            <td>Qwant</td>
            <td><code>!qw privacy tools</code></td>
        </tr>
        <tr>
            <td><code>!brave</code></td>
            <td>Brave Search</td>
            <td><code>!brave secure messaging</code></td>
        </tr>
        <tr>
            <td><code>!w</code></td>
            <td>Wikipedia</td>
            <td><code>!w neural networks</code></td>
        </tr>
        <tr>
            <td><code>!yt</code></td>
            <td>YouTube</td>
            <td><code>!yt cooking tutorials</code></td>
        </tr>
    </tbody>
</table>

### Setting Your Default Search Engine

1. Visit the CogiSearch homepage
2. Scroll down to the Settings section
3. Select an engine from the dropdown or enter a bang for any available search engine
4. Your choice will be saved for future searches

### Adding to Your Browser

To add CogiSearch as a search engine in your browser:

1. Copy this URL: `https://search.cogilabs.eu/?q=%s`
2. In your browser's search engine settings:
  - **Chrome**: Settings → Search Engine → Manage Search Engines → Add
  - **Firefox**: Settings → Search → Add Search Engine → Other
  - **Edge**: Settings → Privacy, Search and Services → Address Bar and Search → Manage Search Engines → Add
3. Name it "CogiSearch" and paste the URL
4. Set it as your default search engine (optional)

## Self-Hosting

CogiSearch is a static website that can be hosted on any web server:

1. Clone the repository: `git clone https://github.com/cogilabs/cogisearch.git`
2. Upload the files to your web server
3. Access the site through your domain

No server-side processing is required as all functionality is client-side JavaScript.

## Customizing

### Adding Custom Bangs

If you host the project yourself, you can add your own custom bangs by editing the `customBangs.js` file:

```javascript
// Add your custom bangs to this array
const customBangs = [
  {
    t: "example",  // Bang trigger (what comes after the !)
    s: "Example Search",  // Display name
    u: "https://example.com/search?q={{{s}}}", // URL with {{{s}}} as the search placeholder
    d: "example.com"  // Domain
  }
];
```

I plan to add a "add your own bangs" feature, but for now, if you use CogiSearch as is, don't hesitate to do a pull request with your custom bangs!

## License

CogiSearch is licensed under the MIT License. See [LICENSE](/LICENSE) for more information.

---

<p align="center">Powered by <a href="https://Cogilabs.eu/">Cogilabs.eu</a></p>
