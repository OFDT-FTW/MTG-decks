# Comment rajouter un deck

1. Copier/coller [template.html](template.html) dans le dossier correspondant au format du deck. Si le dossier n'existe pas, le créer.<br/> 
Pour le nom du fichier, mettre le code de l'extension principale du deck (s'il y en a un), les couleurs utilisées et le nom du deck. Pas besoin d'être ultra strict, le but est de pouvoir facilement savoir quel type de deck est dans le fichier.<br/> 
2. Éditer le fichier créé et modifier
   1. L'image de fond (chercher `url` dans la balise `<style>`)
   2. Remplacer `{DeckTitle}` par le nom du fichier. 
   3. Replacer `{DeckName}` par le nom du deck
   4. Remplacer `{author}` par l'auteur du deck<br/>
   Si pas besoin d'auteur car préconstruit (par exemple), enlever la balise `<div class="row">` et son contenu autour du `{author}`.
   5. Remplacer `{deckstatsLink}` par le lien deckstats.net. Il est générable via Cockatrice en faisant `Éditeur de deck -> Envoyer le deck vers le service en ligne -> Analyser le deck (deckstats.net)`.<br/>
   Si pas envie de mettre un lien là, supprimer la balise `<a>` avec comme `href="{deckstatsLink}"`
   6. Remplacer `{deckCode}` par le code du deck. <br/>
   Il est générable via cockatrice : `Éditeur de deck -> Copier le deck dans le presse-papier -> Avec annotations`.
3. Ouvrir le fichier dans son navigateur pour vérifier que tout s'affiche bien 
4. Commiter et ouvrir la PR vers le repo principal