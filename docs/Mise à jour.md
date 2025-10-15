Reconstruis :
text.
mkdocs build

Vérifie que les avertissements disparaissent ou sont acceptables.


Serve :
text
mkdocs serve

Ouvre http://127.0.0.1:8000/chapitre2 > Confirme cs_formula.png.
Arrête : Ctrl + C.



5. Commite et Pousse sur gh-pages

Ajoute :
textgit add mkdocs.yml docs/

Commite :
textgit commit -m "Correction nav et lien cs_formula.png pour baptême 19 oct"

Pousse :
text
git checkout gh-pages
git merge main
git push origin gh-pages

Username : SurnumerismeAuthor.
Password : Token PAT.


Déploie :
text
ghp-import site -n -p -m "Déploiement pour baptême 19 oct"


6. Vérifie le Site

Attends 1–10 min, ouvre https://surnumerismeauthor.github.io/surnumerisme-livre/chapitre2 (Ctrl + F5).
GitHub Actions : github.com/SurnumerismeAuthor/surnumerisme-livre > Actions > "pages build and deployment" (vert = OK).