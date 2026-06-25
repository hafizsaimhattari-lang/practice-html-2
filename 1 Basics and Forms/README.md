# 📝 1 Basics and Forms - Complete Study Notes

## 📚 Is Folder Ka Maqsad
Is folder mein humne HTML ki bunyadi (basic) cheezon aur Forms ko cover kiya hai. Neeche har ek topic ki mukammal tafseel aur code examples diye gaye hain jo is folder ki files (`1 start.html`, `3 Forms.html`, etc.) mein practice kiye gaye hain.

---

## 🎯 Topic 1: HTML Basics & Text Elements (`1 start.html`)

### 1. Headings & Paragraphs
- **Headings**: HTML mein 6 levels ki headings hoti hain. `<h1>` sabse badi aur `<h6>` sabse choti.
- **Paragraphs**: `<p>` tag text likhne ke liye use hota hai.
- **Line Break**: `<br>` tag se text ko nayi line par laya jata hai.
- **Horizontal Rule**: `<hr>` tag ek horizontal line draw karne ke liye hota hai.

```html
<h1>Heading 1</h1>
<p>Saim is a Good Guy</p>
<hr> <!-- Ek line draw karega -->
<p>Good Guy <br> is Saim</p> <!-- Line break -->
```

### 2. Links & Images (Anchor and Img tags)
- **Anchor `<a href="...">`**: Kisi doosre page ya website ka link banane ke liye.
- **Image `<img src="...">`**: Page par tasveer lagane ke liye.
- **Absolute vs Relative Links**:
  - Absolute: Kisi external website ka poora URL (e.g. `https://google.com`).
  - Relative: Aapke apne computer/folder ka path (e.g. `1 Shahi-Paneer-2.jpg`).

```html
<!-- Absolute Link Example -->
<a href="https://www.dawateislami.net" target="_blank">Visit Website</a>

<!-- Image with Link Example -->
<a href="https://myfoodstory.com/..." target="_blank">
  <img src="1 Shahi-Paneer-2.jpg" height="auto" width="200px" alt="Paneer">
</a>
```

### 3. Text Formatting Tags
HTML mein text ko design ya style dene ke liye yeh tags use hote hain:
- **Bold**: `<b>` (sirf bold) aur `<strong>` (bold aur ahmiyat wala).
- **Italic**: `<i>` (tircha) aur `<em>` (emphasis).
- **Underline**: `<u>` aur `<ins>` (inserted text).
- **Strikethrough**: `<s>` aur `<del>` (delete kiya hua text).
- **Subscript & Superscript**:
  - `<sub>`: Neeche text likhna (e.g., H<sub>2</sub>O) -> `H<sub>2</sub>O`
  - `<sup>`: Oopar text likhna (e.g., a<sup>2</sup>) -> `a<sup>2</sup>`
- **Highlight**: `<mark>` background color highlight ke liye.
- **Pre-formatted**: `<pre>` (Jaise code mein spaces honge, wese hi dikhayega).
- **Abbreviation**: `<abbr title="Full Form">HTML</abbr>`.
- **Keyboard Shortcut**: `<kbd>Ctrl</kbd> + <kbd>C</kbd>`.

### 4. Attributes
- **`style="..."`**: Inline CSS ke liye (e.g., `color: black; background-color: blueviolet;`).
- **`title="..."`**: Tooltip ke liye (jab mouse upar laayein toh text nazar aaye).

---

## 🎯 Topic 2: Forms in HTML (`3 Forms.html`)

Forms user se data lene ke liye istemal hote hain (jaise Login ya Signup forms).

### 1. Form Structure
- **`<form>`**: Main container form ke liye. Iska attribute `action=""` batata hai ke data kahan bhejna hai.
- **`<label>`**: Input field ka naam batane ke liye (e.g., "Username:"). Isme `for="id"` ka attribute use hota hai taake ye input ke sath connect ho sake.

### 2. Input Types
- `<input type="text">`: Simple text likhne ke liye.
- `<input type="password">`: Hidden text (password) ke liye.
- `<input type="checkbox">`: Multiple choices mein se select karne ke liye (Tick mark ✅).
- `<input type="radio">`: Sirf ek option select karne ke liye (Options mein se ek).
- `<input type="button">` / `<button>`: Form ko submit ya click karne ke liye.

### 3. Form Example with Table
Humne `3 Forms.html` mein tables ka use kar ke ek neat form layout banaya:

```html
<form action="https://www.google.com" target="_blank">
    <table>
        <tr>
            <td><label for="username">Username:</label></td>
            <td><input type="text" id="username" placeholder="Enter Username"></td>
        </tr>
        <tr>
            <td><label for="password">Password:</label></td>
            <td><input type="password" id="password" placeholder="Enter Password"></td>
        </tr>
        <tr>
            <td colspan="2"><button>Submit</button></td>
        </tr>
    </table>
</form>
```

### 4. Form without Table
```html
<form>
    <label for="username">UserName:</label>
    <input type="text" placeholder="Enter User Name" id="username">
    <br><br>
    <input type="button" value="Submit">
</form>
```

---

## 💡 Notes
- Code ko read karne ke liye `1 start.html` aur `3 Forms.html` ko VS Code mein kholen aur unki output browser mein dekhein.
- HTML mein Comments `<!-- comment -->` tags ke darmian likhe jate hain. Inline comments ka concept bhi try kiya gaya hai.
