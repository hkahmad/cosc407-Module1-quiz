# COSC407 Quiz

A practice quiz on COSC407 Module 1, *Course Preliminaries & Language Evaluation Criteria*. It has 42 questions in 5 sections. It runs in any browser, and you can install it on a computer or phone as a Progressive Web App (PWA).

## Run it locally
```
python -m http.server 8000
```
Open http://localhost:8000

## Put it online
Upload this folder to any static host, such as GitHub Pages, Netlify or Vercel. Installing needs HTTPS, and all of these hosts provide it.

## Install it
- **Desktop (Chrome/Edge):** click the install icon in the address bar.
- **Android (Chrome):** menu ⋮ → *Install app*.
- **iPhone/iPad (Safari):** Share → *Add to Home Screen*.

Once installed, the app also works offline.

## Add questions (e.g. for Module 2)
Add entries to the `QUESTIONS` array in `index.html`:
```js
{ c: "Section", q: "Question?", o: ["A", "B", "C", "D"], a: 1, e: "Explanation" }
```
`a` is the index of the correct option, counting from 0. The options are shuffled when shown. A new section name shows up in the dropdown automatically.
After you change any file, update `CACHE` in `sw.js` (e.g. `cosc407-quiz-v2`) so installed copies get the new version.
