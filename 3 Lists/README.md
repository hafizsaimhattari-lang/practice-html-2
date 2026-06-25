# 📋 3 Lists in HTML - Complete Study Notes

## 📚 Is Folder Ka Maqsad
HTML mein data ko ek tarteeb (order) ya baghair tarteeb (bullets) ki shakal mein dikhane ke liye Lists ka use kiya jata hai. Is folder ki files (jaise `4 Lists in html.html`) mein 4 kisam ki lists cover ki gayi hain.

---

## 🎯 Topic 1: Unordered Lists (`<ul>`)

Jab items ki tarteeb (numbering) zaroori na ho, toh hum Unordered list banate hain. Isme items ke sath bullets/circles aate hain.

- `<ul>` (Unordered List): List start karne ke liye.
- `<li>` (List Item): List ke andar har naye point ke liye.

```html
<ul>
  <li>Saim</li>
  <li>Talha</li>
  <li>Ali</li>
</ul>
```

---

## 🎯 Topic 2: Ordered Lists (`<ol>`)

Jab items ko ek properly numbered tarteeb deni ho (1, 2, 3 ya A, B, C).

- `<ol>` (Ordered List): Isme aap `type` attribute de kar style change kar sakte hain.
- `type="1"`: Numbers (Default)
- `type="A"`: Capital Alphabets
- `type="a"`: Small Alphabets
- `type="i"`: Roman Numerals

```html
<ol type="A">
  <li>Saim</li>
  <li>Talha</li>
</ol>
<!-- Output:
 A. Saim
 B. Talha 
-->
```

---

## 🎯 Topic 3: Description List (`<dl>`)

Agar aapko kisi cheez ka naam likhna ho aur uske neeche uski description (tafseel) deni ho, toh Description List use hoti hai.

- `<dl>` (Description List): Main container.
- `<dd>` (Description Data / Term): Jis cheez ko define karna ho.
- `<dt>` (Description Term Details): Uski details ya tafseel.

```html
<dl>
  <dd><mark>HTML</mark></dd>
  <dt>Hyper Text Markup Language</dt>
</dl>
```

---

## 🎯 Topic 4: Nested Lists 

Ek list ke andar doosri list banane ko Nested List kehte hain. Yeh drop-downs ya sub-categories banane ke liye bohat kaam aati hai.

### Example:
Ek `<ul>` (Main List) ke kisi ek `<li>` ke andar doosra `<ul>` ya `<ol>` shuru kar dena.

```html
<ul>
  <li>
    <h2>Fruit</h2>
    <ul>
      <li>Apple</li>
      <li>Mango</li>
    </ul>
  </li>
  
  <li>
    <h2>Vegetables</h2>
    <ul>
      <li>Aaloo</li>
      <li>Onion</li>
    </ul>
  </li>
</ul>
```

---

## 💡 Notes
- VS Code Shortcut: Aap `li*5` likh kar Enter dabayen toh khud hi 5 `<li>` tags ban jayenge.
- Aap Ordered (`<ol>`) ke andar Unordered (`<ul>`) aur vice versa dono ka nested combinations bana sakte hain jaisa ke `4 Lists in html.html` mein practice kiya gaya hai.
