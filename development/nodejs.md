# Titre de la compétence

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- Comment développer en utilisant un système de *livereloading* (`nodemon` par exemple) ✔️
- La connexion de mon application à une base de données avec et sans ORM/ODM (avec `mongodb` puis `mongoose` par exemple) ✔️
- Le développement d'une API REST et GraphQL (avec les packages `express` et `graphql` par exemple) ✔️
- *Bonus : la manipulation des fichiers système avec `fs` et l'utilisation des streams en NodeJS* ✔️

## 💻 J'utilise

### Un exemple personnel commenté ❌ / ✔️

```javascript
// This function is used inside a TypeGraphql nodejs API and will take a string name 'code' as parameter and write the contents of that string to a new file stored locally
// It will then use a node command to execute the file and return the respnse as a string

async postCode(@Arg("code") code: string): Promise<string> {
    try {
      fs.writeFile("./src/child-processes/code.js", code);
    } catch {
      console.warn("error save file !");
    }
    const response = await execShellCommand(
      "node ./src/child-processes/code.js",
    );
    return response.replace("/n", "");
  }
```

### Utilisation dans un projet ✔️

[lien github](https://github.com/WildCodeSchool/2209-wns-rivest-groupe4-back)

Description :

### Utilisation en production si applicable❌ / ✔️

[lien du projet](...)

Description :

### Utilisation en environement professionnel ❌ / ✔️

Description :

## 🌐 J'utilise des ressources

### Titre

- lien
- description

## 🚧 Je franchis les obstacles

### Point de blocage ❌ / ✔️

Description:

Plan d'action : (à valider par le formateur)

- action 1 ❌ / ✔️
- action 2 ❌ / ✔️
- ...

Résolution :

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
