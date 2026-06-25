# 💬 4 Blockquote and Quotes - Complete Study Notes

## 📚 Is Folder Ka Maqsad
Is folder mein humne HTML mein Quotes (Haqwal / Qoul) aur references likhne ke tags par practice ki hai. Agar aap kisi doosri website, kitaab, ya shakhsiyat ka koi quote apni website par dikhana chahte hain, toh uske liye makhsoos HTML tags use hote hain taake unki formatting alag nazar aaye.

---

## 🎯 Topic 1: Blockquote (`<blockquote>`)

Jab aap kisi doosre source se koi lamba quote (multiple lines wala) copy kar ke lagate hain toh `<blockquote>` tag ka istemal hota hai. 
Browser isko aam taur par thoda indent (left side se margin de kar) show karta hai taake ye aam text se alag nazar aaye.

```html
<blockquote>
    Display quotes that set themselves apart from the rest of your textual content in a striking manner. All you need to do is provide the quote and stylize the text the way you desire.
</blockquote>
```

---

## 🎯 Topic 2: Inline Quote (`<q>`)

Jab aapne kisi ka koi chota sa sentence ya lafaz quote karna ho jo line ke darmian mein hi aaye, toh hum `<q>` tag ka use karte hain. 
Browser iske dono taraf khud ba khud quotation marks (`" "`) laga deta hai.

```html
<p>
    Saim said, <q>HTML is very easy to learn!</q>
</p>
```
*(Yahan HTML is very easy to learn! ke gird quotes khud ban jayenge)*

---

## 🎯 Topic 3: Citation (`<cite>`)

Jab aap quote ka source batate hain (jese kisi ka naam, kitaab ka naam, ya website ka naam) toh usko `<cite>` tag mein likha jata hai. 
Browser isko aam taur par *Italic* (tircha) show karta hai.

```html
<cite> - Lorem ipsum dolor sit amet. <a href="https://www.codehelp.in">ClickHere</a></cite>
```

---

## 💡 Notes
- Practice file `1 blockquote.html` mein in teeno tags (`<blockquote>`, `<q>`, aur `<cite>`) ka combination use kar ke dikhaya gaya hai.
- Aap CSS ki madad se `<blockquote>` ko mazeed behtar (borders, background color, italic text) de kar style bhi kar sakte hain.
