# Tableau Math

Tableau blanc de mathématiques pensé pour une séance en visioconférence : écriture directe au clavier, insertion de symboles par clic et notation vectorielle accessible.

## Fonctionnalités

- **Édition directe** : écrire dans le tableau, sans afficher de code LaTeX.
- **Bibliothèque de symboles** : bases, fractions empilées avec barre horizontale, vecteurs, puissances/indices/racines, alphabet grec et relations.
- **Vecteurs personnalisés** : crée un vecteur avec le nom de ton choix (par exemple MN, w ou u₁), sans être limité à la bibliothèque prédéfinie.
- **Coordonnées en colonne** : crée un vecteur en 2D ou 3D avec les coordonnées saisies, affichées verticalement entre crochets.
- **Vecteurs mis en évidence** : les symboles de la bibliothèque et les vecteurs personnalisés affichent une flèche dessinée au-dessus du nom.
- **Copie texte** : copie une notation mathématique Unicode, pas du LaTeX brut. Les coordonnées en colonne utilisent des crochets Unicode et des retours à la ligne.
- **Copie texte + rendu** : place du texte brut et du HTML mis en forme dans le presse-papiers lorsque le navigateur autorise l'écriture enrichie.
- **Annulation** : bouton et raccourci Ctrl/Cmd + Z.
- **Sauvegarde automatique locale** : le tableau est restauré depuis le stockage du navigateur sur le même appareil.
- **Responsive** : interface utilisable sur ordinateur, tablette et mobile.

Les fractions sont affichées avec un numérateur au-dessus d'une barre horizontale et un dénominateur en dessous. Dans la copie en texte brut, elles deviennent une écriture linéaire telle que 1/2. Le texte brut utilise une flèche combinante Unicode pour représenter les vecteurs personnalisés (par exemple u⃗). Les vecteurs de coordonnées sont rendus en colonne dans le tableau et convertis en notation à crochets Unicode avec des lignes séparées lors de la copie texte. La copie enrichie conserve autant que possible le rendu en colonne et les flèches dessinées au-dessus des noms lorsque l'application de destination accepte le HTML mis en forme. Les navigateurs qui ne prennent pas en charge la copie enrichie retombent sur le texte Unicode.

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
