
This is explaination vedio 
HERE, this is the link:-  https://drive.google.com/drive/folders/1L-GenRUpSQ0baZ98EQ3fSd3E1zmd-KcJ?usp=sharing
  
  
# 🛍️ My Product Store

A responsive and dynamic **Product Listing Website** built using **HTML, CSS, JavaScript, and TypeScript**.

This project fetches product data from an API and dynamically generates product cards on the webpage. It was created to practice working with **arrays, objects, loops, Fetch API, JSON data, DOM manipulation, template literals, and responsive CSS layouts**.

---

## 📌 Project Overview

**My Product Store** is a product listing website where product information is fetched dynamically from the [DummyJSON Products API](https://dummyjson.com/products).

Instead of manually creating individual product cards in HTML, the products are generated dynamically using JavaScript/TypeScript.

The project demonstrates how API data can be:

1. Fetched from an external API
2. Stored in a JavaScript/TypeScript variable
3. Accessed through an array of objects
4. Iterated using `forEach()`
5. Used to generate dynamic HTML
6. Inserted into the DOM
7. Displayed in a responsive product grid

---

## 🎯 Project Objective

The main objective of this project is to understand how **HTML, CSS, JavaScript, TypeScript, APIs, and the DOM** work together to create a dynamic website.

### Concepts practiced

- Arrays
- Arrays of objects
- JavaScript objects
- Object properties
- `for` loops
- `forEach()`
- Arrow functions
- Template literals
- Fetch API
- Promises
- JSON data
- DOM manipulation
- `getElementById()`
- `innerHTML`
- TypeScript
- TypeScript compilation
- Responsive CSS
- CSS Grid / Flexbox

---

## ✨ Features

### Header

The website contains a clean navigation header with:

- **My Product Store** website name
- Home
- Products
- About

### Dynamic Product Cards

Every product card is generated dynamically from API data.

Each card displays:

- 🖼️ Product image
- 🏷️ Product title
- 📝 Product description
- 💰 Product price
- 📉 Discount percentage
- 📂 Product category
- ⭐ Product rating
- 📦 Product stock

### Product Count

The website also displays the total number of products received from the API.

### Responsive Design

The product layout is responsive and adapts to:

- 📱 Mobile devices
- 📱 Tablets
- 💻 Desktop screens

### Hover Effect

Product cards include a hover effect to make the interface more interactive.

---

## 🌐 API

The project uses the DummyJSON Products API:

**API Endpoint:**

`https://dummyjson.com/products`

The API returns product information in JSON format.

The response contains a `products` array containing multiple product objects.

Example structure:

```json
{
  "products": [
    {
      "id": 1,
      "title": "Product Name",
      "description": "Product description",
      "price": 100,
      "discountPercentage": 10,
      "rating": 4.5,
      "stock": 50,
      "category": "category-name",
      "thumbnail": "image-url"
    }
  ]
}
```

---

## 📁 Project Structure

```text
MyProductStore-Project/
│
├── index.html
│
├── css/
│   └── style.css
│
├── js/
│   └── script.js
│
└── assets/
    └── ts/
        └── script.ts
```

### File Description

| File | Purpose |
|---|---|
| `index.html` | Website structure |
| `css/style.css` | Website styling and responsive layout |
| `js/script.js` | Compiled JavaScript used by the browser |
| `assets/ts/script.ts` | TypeScript source code |

---

## ⚙️ How the Project Works

### 1. HTML Structure

The HTML file provides the basic structure of the website.

A dedicated product container is created where JavaScript will insert the dynamically generated product cards.

Example:

```html
<div id="product-container"></div>
```

---

### 2. Selecting the Product Container

The container is accessed using:

```typescript
let productContainer = document.getElementById(
    "product-container"
) as HTMLElement;
```

Here:

- `document.getElementById()` finds the HTML element.
- `"product-container"` is the element's ID.
- `productContainer` stores the selected element.
- `as HTMLElement` tells TypeScript to treat the returned element as an `HTMLElement`.

---

### 3. Fetching API Data

The Fetch API is used to request product data from DummyJSON.

The API response is converted into JSON so that JavaScript/TypeScript can work with the product objects.

Conceptually:

```text
API
 ↓
fetch()
 ↓
Response
 ↓
JSON
 ↓
products array
```

---

### 4. Accessing the Products Array

After receiving the JSON data, the `products` array is accessed and stored in a variable.

This array contains multiple product objects.

Conceptually:

```text
products
 ├── product 1
 ├── product 2
 ├── product 3
 ├── product 4
 └── ...
```

---

### 5
