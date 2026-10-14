# Tableau Math

Tableau blanc de mathématiques pensé pour une séance en visioconférence : écriture directe au clavier, insertion de symboles par clic et notation vectorielle accessible.

## Fonctionnalités

- **Édition directe** : écrire dans le tableau, sans afficher de code LaTeX.
- **Bibliothèque de symboles** : bases, fractions empilées avec barre horizontale, vecteurs, puissances/indices/racines, alphabet grec et relations.
- **Outils vecteurs intégrés à la bibliothèque** : les outils de création sont regroupés dans l'onglet « Outils » au même endroit que les symboles.
- **Vecteurs personnalisés** : crée un vecteur avec le nom de ton choix (par exemple MN, w ou u₁), sans être limité à la bibliothèque prédéfinie.
- **Coordonnées en ligne** : insère les coordonnées sous la forme `(x, y)` en 2D ou `(x, y, z)` en 3D, sur la même ligne que le texte.
- **Modification directe** : double-clique sur un vecteur ou un tuple de coordonnées dans le tableau pour modifier son nom, ses coordonnées ou sa dimension sans le supprimer et le recréer.
- **Vecteurs mis en évidence** : les symboles de la bibliothèque et les vecteurs personnalisés affichent une flèche dessinée au-dessus du nom.
- **Copie texte** : copie une notation mathématique Unicode, pas du LaTeX brut. Les coordonnées utilisent la notation en ligne, par exemple `(2, -1, 3)`.
- **Copie texte + rendu** : place du texte brut et du HTML mis en forme dans le presse-papiers lorsque le navigateur autorise l'écriture enrichie.
- **Annulation** : bouton et raccourci Ctrl/Cmd + Z.
- **Sauvegarde automatique locale** : le tableau est restauré depuis le stockage du navigateur sur le même appareil.
- **Responsive** : interface utilisable sur ordinateur, tablette et mobile.

Les fractions sont affichées avec un numérateur au-dessus d'une barre horizontale et un dénominateur en dessous. Dans la copie en texte brut, elles deviennent une écriture linéaire telle que 1/2. Le texte brut utilise une flèche combinante Unicode pour représenter les vecteurs personnalisés (par exemple u⃗). Les coordonnées des vecteurs sont rendues en ligne dans le tableau et la copie, par exemple `(2, -1, 3)`. La copie enrichie conserve autant que possible le style visuel des vecteurs lorsque l'application de destination accepte le HTML mis en forme. Les navigateurs qui ne prennent pas en charge la copie enrichie retombent sur le texte Unicode.

## Développement local

Aucun installateur, framework ou compilation n'est nécessaire. Ouvrir index.html dans un navigateur. Pour un comportement du presse-papiers plus proche de la production, utiliser un serveur local ou localhost, car certains navigateurs limitent l'accès au presse-papiers hors contexte sécurisé.

## Déploiement sur Vercel

1. Importer ce dépôt GitHub dans Vercel.
2. Choisir **Other** comme framework si Vercel demande de le préciser.
3. Laisser la commande de build vide.
4. Déployer le répertoire racine du dépôt, où se trouve index.html.

Le site est statique et n'a pas besoin de variables d'environnement, d'API, ni de configuration serveur.

## Confidentialité

Le contenu du tableau est sauvegardé dans localStorage du navigateur. Il n'est pas envoyé à un serveur par cette application. Effacer les données du site dans le navigateur supprime aussi cette sauvegarde.
