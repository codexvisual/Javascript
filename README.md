# Javascript<div align="center">

# ⚡ Ultimate JavaScript Cheat Sheet

**Variables · Functions · Arrays · ES6 · Async · DOM**  
_Every modern JS concept in one place_

[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![ES6+](https://img.shields.io/badge/ES6+-blue?style=for-the-badge)](https://www.ecma-international.org/)

</div>

---

## 📦 1. Variables & Data Types (ভেরিয়েবল ও ডেটা টাইপ)

<div align="center">

| Code | Description |
|------|-------------|
| `var x = 10;` | পুরনো স্টাইল (function-scoped) |
| `let y = 20;` | ব্লক-স্কোপড, পরিবর্তনযোগ্য |
| `const PI = 3.1416;` | ব্লক-স্কোপড, অপরিবর্তনীয় |
| `typeof x;` | টাইপ চেক (`"number"`, `"string"`, `"object"`) |
| **Primitive types:** `string`, `number`, `boolean`, `null`, `undefined`, `symbol`, `bigint` | |

</div>

---

## ➕ 2. Operators (অপারেটর)

<div align="center">

| Operator | Description |
|----------|-------------|
| `+`, `-`, `*`, `/`, `%` | গাণিতিক |
| `==`, `===` | সমান (টাইপসহ `===`) |
| `!=`, `!==` | অসমান |
| `>`, `<`, `>=`, `<=` | তুলনা |
| `&&`, `\|\|`, `!` | লজিক্যাল (AND, OR, NOT) |
| `++`, `--` | ইনক্রিমেন্ট/ডিক্রিমেন্ট |

</div>

---

## 🔀 3. Control Flow (কন্ডিশন ও লুপ)

<div align="center">

| Code | Description |
|------|-------------|
| `if (condition) { ... } else { ... }` | কন্ডিশন |
| `switch(x) { case 1: ... break; default: ... }` | সুইচ স্টেটমেন্ট |
| `for (let i=0; i<5; i++) { ... }` | ফর লুপ |
| `while (condition) { ... }` | হোয়াইল লুপ |
| `do { ... } while (condition);` | ডু-হোয়াইল |
| `for (let item of array) { ... }` | ফর-অফ (অ্যারে) |
| `for (let key in object) { ... }` | ফর-ইন (অবজেক্ট) |

</div>

---

## 🛠️ 4. Functions (ফাংশন)

<div align="center">

| Code | Description |
|------|-------------|
| `function greet(name) { return "Hello " + name; }` | সাধারণ ফাংশন |
| `const greet = (name) => "Hello " + name;` | অ্যারো ফাংশন (ES6) |
| `const sum = (a, b) => a + b;` | ইমপ্লিসিট রিটার্ন |
| `greet("Rahim");` // → "Hello Rahim" | ফাংশন কল |
| `function add(a, b=5) { ... }` | ডিফল্ট প্যারামিটার |

</div>

---

## 📚 5. Arrays (অ্যারে)

<div align="center">

| Method | Description |
|--------|-------------|
| `let arr = [1, 2, 3];` | তৈরি |
| `arr.push(4);` | শেষে যোগ |
| `arr.pop();` | শেষ থেকে বাদ |
| `arr.unshift(0);` | শুরুতে যোগ |
| `arr.shift();` | শুরু থেকে বাদ |
| `arr.map(x => x*2);` | নতুন অ্যারে, রূপান্তরিত |
| `arr.filter(x => x > 1);` | শর্তপূরণকারী ফিল্টার |
| `arr.reduce((sum, x) => sum + x, 0);` | জমা করা |
| `arr.forEach(x => console.log(x));` | প্রতিটি এলিমেন্টে কাজ |
| `arr.find(x => x > 2);` | প্রথম শর্তপূরণকারী |
| `arr.includes(3);` | আছে কিনা (true/false) |
| `arr.slice(1, 3);` | অংশ কাটা |
| `arr.splice(1, 1, "new");` | মুছা/যোগ করা |

</div>

---

## 🧵 6. Strings (স্ট্রিং)

<div align="center">

| Method | Description |
|--------|-------------|
| `str.length` | দৈর্ঘ্য |
| `str.toUpperCase()` | বড় হাতের |
| `str.toLowerCase()` | ছোট হাতের |
| `str.trim()` | দুই পাশের স্পেস সরানো |
| `str.includes("hello")` | আছে কিনা |
| `str.indexOf("world")` | অবস্থান (-1 না পেলে) |
| `str.replace("old", "new")` | প্রতিস্থাপন |
| `str.split(",")` | অ্যারেতে ভাঙা |
| `` `Hello ${name}` `` | টেমপ্লেট লিটারেল (ES6) |

</div>

---

## 🧱 7. Objects (অবজেক্ট)

<div align="center">

| Code | Description |
|------|-------------|
| `const obj = { name: "Rahim", age: 25 };` | অবজেক্ট তৈরি |
| `obj.name` / `obj["age"]` | মান পড়া |
| `obj.job = "Dev";` | নতুন প্রপার্টি যোগ |
| `delete obj.age;` | প্রপার্টি মুছা |
| `Object.keys(obj)` | সব কী-এর অ্যারে |
| `Object.values(obj)` | সব ভ্যালুর অ্যারে |
| `Object.entries(obj)` | কী-ভ্যালু পেয়ার অ্যারে |
| `const { name, age } = obj;` | ডিস্ট্রাকচারিং (ES6) |

</div>

---

## 🌐 8. DOM Manipulation (DOM নিয়ন্ত্রণ)

<div align="center">

| Code | Description |
|------|-------------|
| `document.querySelector(".class")` | প্রথম এলিমেন্ট সিলেক্ট |
| `document.querySelectorAll("div")` | সবগুলো সিলেক্ট (নোডলিস্ট) |
| `document.getElementById("id")` | আইডি দিয়ে সিলেক্ট |
| `el.textContent = "Hello";` | টেক্সট পরিবর্তন |
| `el.innerHTML = "<p>Hi</p>";` | HTML সেট |
| `el.style.color = "red";` | স্টাইল পরিবর্তন |
| `el.classList.add("active");` | ক্লাস যোগ |
| `el.classList.remove("active");` | ক্লাস বাদ |
| `el.classList.toggle("dark");` | টগল |
| `document.createElement("div");` | নতুন এলিমেন্ট |
| `parent.appendChild(child);` | চাইল্ড যোগ |
| `parent.removeChild(child);` | চাইল্ড বাদ |

</div>

---

## 🎧 9. Events (ইভেন্ট)

<div align="center">

| Code | Description |
|------|-------------|
| `el.addEventListener("click", myFunction);` | ইভেন্ট লিসেনার |
| `el.removeEventListener("click", myFunction);` | লিসেনার বাতিল |
| `event.preventDefault()` | ডিফল্ট অ্যাকশন বন্ধ |
| `event.stopPropagation()` | বাবলিং বন্ধ |
| Common events: `click`, `submit`, `keydown`, `mouseover`, `load`, `input` | |

</div>

---

## ⏳ 10. Async JavaScript (অ্যাসিঙ্ক)

<div align="center">

| Code | Description |
|------|-------------|
| `setTimeout(() => { ... }, 1000);` | নির্দিষ্ট সময় পর একবার |
| `setInterval(() => { ... }, 1000);` | নির্দিষ্ট সময় পরপর |
| `fetch("url")` | API কল (Promise) |
| `fetch("url").then(res => res.json()).then(data => {})` | Promise চেইন |
| `async function getData() { const res = await fetch("url"); }` | async/await (ES8) |
| `try { ... } catch(err) { console.log(err); }` | এরর হ্যান্ডলিং |
| `new Promise((resolve, reject) => { ... })` | Promise তৈরি |

</div>

---

## 💾 11. Storage & JSON

<div align="center">

| Code | Description |
|------|-------------|
| `JSON.stringify(obj)` | অবজেক্ট → স্ট্রিং |
| `JSON.parse(str)` | স্ট্রিং → অবজেক্ট |
| `localStorage.setItem("key", "value");` | ডাটা সেভ |
| `localStorage.getItem("key");` | ডাটা পড়া |
| `localStorage.removeItem("key");` | ডাটা মুছা |

</div>

---

<div align="center">

### ⚡ Master JavaScript with these snippets – everything you need, right here!  
**Happy Coding!**

[![Profile Views](https://komarev.com/ghpvc/?username=your-username&color=yellow&style=flat-square)](https://github.com/your-username)

</div>
