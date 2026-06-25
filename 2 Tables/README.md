# 📊 2 Tables and Spans - Complete Study Notes

## 📚 Is Folder Ka Maqsad
Is folder mein humne HTML Tables banana aur unhein style karna seekha hai. Isme basic tables se le kar complex tables (jisme rows aur columns aapas mein merge hote hain) ki mukammal tafseel mojood hai.

---

## 🎯 Topic 1: Basic HTML Tables (`Class 3 1 table.html`)

HTML mein data ko rows aur columns (grid) ki shakal mein dikhane ke liye `<table>` tag ka istemal hota hai.

### Important Tags:
- `<table>`: Main container jo table banata hai.
- `<tr>` (Table Row): Ek nayi row (horizontal line) shuru karne ke liye.
- `<th>` (Table Heading): Table ki headings (columns ke naam) ke liye. Yeh text ko bold aur center karta hai.
- `<td>` (Table Data): Table ke andar ka actual data ya cell.
- `<caption>`: Table ka title dene ke liye.

### Thead, Tbody, aur Tfoot (Rowgroups)
Ek achi practice yeh hai ke table ko teen hisson mein taqseem kiya jaye (Row grouping):
1. **`<thead>`**: Table ka heder section (isme headings aati hain).
2. **`<tbody>`**: Table ka main body (isme asli data aata hai).
3. **`<tfoot>`**: Table ka footer (yahan normally total waghera aata hai).

```html
<table>
    <thead>
        <tr>
            <th>Month</th>
            <th>Amount</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Jan</td>
            <td>100</td>
        </tr>
    </tbody>    
    <tfoot>
       <tr>
        <td>Total</td>
        <td>100</td>
       </tr>
    </tfoot>   
</table>
```

---

## 🎯 Topic 2: Colspan aur Rowspan (`class 3 2 span.html`)

Agar aap chahte hain ke table ka ek cell multiple rows ya columns ki jagah le, toh hum `colspan` ya `rowspan` use karte hain.

> **Rule:** `rowspan` ya `colspan` kabhi bhi khud se nayi rows ya columns paida (create) nahi karte. Ye sirf pehle se mojood rows/columns ke andar apni jagah gherte hain.

### 1. Colspan (Columns merge karna)
Jab ek cell ko horizontal (left to right) spread karna ho.
```html
<!-- Yeh heading do (2) columns ki jagah ghere gi -->
<th colspan="2">Month</th>
```

### 2. Rowspan (Rows merge karna)
Jab ek cell ko vertical (top to bottom) spread karna ho.
```html
<!-- Yeh data do (2) rows ki jagah ghere ga -->
<td rowspan="2">State of Health</td>
```

---

## 🎯 Topic 3: Colgroup aur Col (`class 3 7 colgroup&rowgroup.html`)

Agar aapko table ke poore column ko ek saath style karna ho (maslan uska background color change karna ho) toh har `<td>` mein ja kar style likhna mushkil hota hai. Iske liye `<colgroup>` use hota hai.

- `<colgroup>`: Columns ki grouping ke liye container.
- `<col>`: Individual column ko style karne ke liye.
- `span="n"`: Ek hi style ko n columns par apply karne ke liye.

```html
<table>
    <!-- Pehla column Purple hoga -->
    <!-- Agle teen (3) columns Blue honge -->
    <!-- Aakhri column Red hoga -->
    <colgroup>
        <col span="1" style="background-color:purple;">
        <col span="3" style="background-color:blue;">
        <col span="1" style="background-color:red">
    </colgroup>
    
    <tr>
        <th>Col 1</th>
        <th>Col 2</th>
        <th>Col 3</th>
        <th>Col 4</th>
        <th>Col 5</th>
    </tr>
</table>
```

---

## 💡 Notes
- Practice files (`class 3 4 football scores span.html` aur `class 3 6 product sales colgroup practice.html`) mein in sab concepts ka behtareen use kiya gaya hai.
- CSS properties jaise `border-collapse: collapse;` use kar ke table ke borders ko neat banaya jata hai.
