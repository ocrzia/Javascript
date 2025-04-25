# 🌟 Repo Global FullStack Js - Javascript

Récap de tout ce qu'on a déjà vu ensemble en Javascript 

## Nos exercices
1. [Compteur / Dark Mode](https://github.com/ocrzia/JS1--Compteur-darkmode)
2. [Conditions](https://github.com/ocrzia/JS2--Conditions)
3. [Pair & Impair](https://github.com/ocrzia/JS3--Pair-impair)
4. [Random Number](https://github.com/ocrzia/JS4-Random-number)

## 1. Tableaux (`Array`)

<!-- ### Méthodes de base
- **push()** : Ajoute un élément à la fin du tableau.
- **pop()** : Retire le dernier élément.
- **shift()** : Retire le premier élément.
- **unshift()** : Ajoute un élément au début.

### Itération et transformation
- **forEach()** : Exécute une fonction sur chaque élément.
- **map()** : Crée un nouveau tableau transformé.
- **filter()** : Garde les éléments qui passent un test.
- **find()** : Renvoie le premier élément qui passe un test.

### Recherche et manipulation
- **includes()** : Vérifie si un élément est présent.
- **indexOf()** : Renvoie l’index d’un élément.
- **slice()** : Extrait une portion (sans modifier le tableau).
- **splice()** : Ajoute ou supprime des éléments (modifie le tableau).

### Autres
- **join()** : Transforme en chaîne de caractères.
- **sort()** : Trie les éléments.
- **reverse()** : Inverse l’ordre des éléments. -->

---

## 2. Chaînes de caractères (`String`)

<!-- ### Propriétés et méthodes
- **length** : Longueur de la chaîne.
- **charAt(index)** : Caractère à une position donnée.
- **includes()** : Vérifie si une sous-chaîne est présente.
- **indexOf()** / **lastIndexOf()** : Position d’un caractère ou mot.
- **slice()**, **substring()** : Extraient des portions de chaîne.
- **toLowerCase()** / **toUpperCase()** : Minuscule / Majuscule.
- **replace()** : Remplace une partie de la chaîne.
- **split()** : Découpe une chaîne en tableau.
- **trim()** : Supprime les espaces avant/après. -->

---

## 3. Nombres (`Number`)

<!-- ### Méthodes
- **toFixed()** : Fixe le nombre de décimales (retourne une chaîne).
- **toString()** : Convertit en chaîne.
- **toPrecision()** : Arrondit avec précision globale.

### Méthodes globales
- **Number.isNaN()**, **Number.isInteger()**, **Number.isFinite()** : Vérifications de validité. -->

---

## 4. Objet [Math](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math)

### Méthodes mathématiques
- **Math.round()**, **Math.floor()**, **Math.ceil()**
- **Math.random()** : Nombre pseudo-aléatoire entre 0 et 1.
<!-- - **Math.max()**, **Math.min()** -->
<!-- - **Math.abs()**, **Math.pow()**, **Math.sqrt()** -->

---

## 5. Dates (`Date`)

<!-- ### Lecture de date
- **getFullYear()**, **getMonth()**, **getDate()**
- **getDay()**, **getHours()**, **getMinutes()**, **getSeconds()**

### Formatage
- **toLocaleDateString()** : Format lisible.
- **toISOString()** : Format ISO. -->

---

## 6. Objets (`Object`)

<!-- ### Méthodes natives
- **Object.keys()**, **Object.values()**, **Object.entries()**
- **hasOwnProperty()**
- **JSON.stringify()** : Objet vers JSON.
- **JSON.parse()** : JSON vers objet. -->

---


# DOM – Manipulation des éléments HTML

## 🔍 Sélection d’éléments
- **document.getElementById("id")** : sélectionne par l'ID
- **document.querySelector("selector")** : sélectionne le premier élément qu'il rencontre par le sélecteur CSS indiqué (attention à bien indiquer . & #)
- **document.querySelectorAll("selector")** : sélectionne la collection des éléments par le sélecteur CSS indiqué
- **element.closest("selector")** : cherche l'élément le plus proche du sélecteur (dans sa hiérarchie parentale)

## ➕ Ajout ou suppression d’éléments
- **element.appendChild(nouvelElement)** : ajoute un enfant
- **element.append(nouvelElement)** : ajoute à la fin (string ou élément)
- **element.prepend(nouvelElement)** : ajoute au début
- **element.remove()** : supprime l’élément lui-même 

## 📋 Gestion des attributs
- **element.getAttribute("attribut")** : va rechercher la valeur de l'attribut sélectionné
- **element.setAttribute("attribut", "valeur")** : met l'attribut sélectionné à une certaine valeur
- **element.hasAttribute("attribut")** : vérifie si l'élément à l'attribut sélectionné
- **element.removeAttribute("attribut")** : enlève l'attribut sélectionné

## 🧭 Navigation dans le DOM
- **element.parentElement** : va chercher le parent direct de l'élément sélectionné
- **element.children** : va chercher la collection de tous les enfants directs de l'élément sélectionné
- **element.nextElementSibling** : va chercher l'élément frère/soeur qui suit directement l'élément sélectionné
- **element.previousElementSibling** : va chercher l'élément frère/soeur qui précède directement l'élément sélectionné

## Propriétés DOM fréquentes

### Contenu texte/HTML
- **innerText** : Texte visible. [MDN](https://developer.mozilla.org/fr/docs/Web/API/HTMLElement/innerText)
- **textContent** : Texte brut (même caché). [MDN](https://developer.mozilla.org/en-US/docs/Web/API/Node/textContent)
- **innerHTML** : Contenu HTML interne. [MDN](https://developer.mozilla.org/fr/docs/Web/API/Element/innerHTML)
- **outerHTML** : HTML complet (la balise incluse). [MDN](https://developer.mozilla.org/fr/docs/Web/API/Element/outerHTML) 

### Formulaires et attributs
- **value** : Valeur d’un champ (`input`, etc.).
- **checked** : Si coché (checkbox/radio).
- **disabled** : Si désactivé.
- **href**, **src** : Pour les liens, images, vidéos.

### Identifiants et classes
- **id** : Identifiant.
- **className** : Classes en texte.
- **classList** : Liste de classes manipulables.

### Style et données
- **style** : Accès au style inline (`element.style.color`, etc.).
- **dataset** : Données `data-*` (ex: `element.dataset.id`).