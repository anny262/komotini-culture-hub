# komotini-culture-hub
Skeleton repo – will be filled from github.dev editor.

## Πώς το μετατρέπω σε Drupal Theme

1. **`drupal theme:generate`** (Drupal Console) → νέο custom theme `kch`.
2. Αντιγράφω το περιεχόμενο του `index.html` σε `templates/page.html.twig`,
   σπάζω header / footer σε `block--header.html.twig`, `block--footer.html.twig`.
3. Δημιουργώ `scss/main.scss` + `js/app.js` μέσα στο theme.
4. Δηλώνω τα assets στο **`kch.libraries.yml`**:
   ```yml
   global-styling:
     version: 1.x
     css:
       theme:
         css/main.css: {}
     js:
       js/app.js: {}
5.Ενεργοποιώ το theme, τρέχω npm run build (Sass → CSS)
και καθαρίζω cache (drush cr). Το demo εμφανίζεται μέσα στο Drupal.
