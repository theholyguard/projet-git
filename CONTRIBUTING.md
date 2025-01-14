# Guide de Contribution

Merci de vouloir contribuer à ce projet ! Ce guide détaille les étapes pour soumettre des contributions et les bonnes pratiques à respecter.

---

## **Comment Contribuer**

### **1. Forker le dépôt**
Créez une copie du projet sur votre compte GitHub en cliquant sur le bouton **Fork**.

### **2. Cloner votre fork**
Clonez le dépôt forké sur votre machine locale :
```bash
git clone git@github.com:VOTRE-USERNAME/REPOSITORY.git
cd REPOSITORY
```

### **3. Configurer les remotes**
Ajoutez le dépôt d'origine comme remote pour garder votre fork à jour :
```bash
git remote add upstream git@github.com:ORIGINAL-USERNAME/REPOSITORY.git
```

Pour vérifier les remotes configurées :
```bash
git remote -v
```

### **4. Créer une branche pour votre contribution**
Créez une branche descriptive à partir de la branche `develop` ou `main` :
```bash
git checkout -b feature/nom-de-la-branche
```

- **Pour une nouvelle fonctionnalité** : utilisez `feature/` comme préfixe (e.g., `feature/ajout-auth`).
- **Pour corriger un bug** : utilisez `bugfix/` comme préfixe (e.g., `bugfix/correction-affichage`).

---

## **Bonnes Pratiques de Contribution**

### **1. Respecter le style de code**
- Suivez les conventions définies dans le projet (par exemple : ESLint, Prettier, etc.).
- Exécutez les tests et le linter localement avant de soumettre votre code :
  ```bash
  npm run lint
  npm run test
  ```

### **2. Écrire des messages de commit clairs**
Rédigez des messages de commit précis et concis, en anglais ou français, suivant le format :
```
[Type]: Description concise

Exemple :
feat: Add user authentication system
fix: Correct footer alignment issue
docs: Update README with setup instructions
```

Types courants :
- `feat`: Nouvelle fonctionnalité.
- `fix`: Correction de bug.
- `docs`: Documentation.
- `style`: Modifications de style (CSS, indentations).
- `test`: Ajout ou correction de tests.

### **3. Ajouter des tests**
- Pour toute nouvelle fonctionnalité, ajoutez des tests.
- Vérifiez que votre code passe tous les tests existants.

### **4. Documenter vos modifications**
- Si vous ajoutez une fonctionnalité, mettez à jour la documentation correspondante (e.g., `README.md`).
- Si votre code introduit des dépendances, expliquez comment les installer.

---

## **Mettre à jour votre fork**
Avant de commencer à travailler sur une nouvelle branche, mettez à jour votre fork pour éviter les conflits :
```bash
git checkout develop
git pull upstream develop
git push origin develop
```

---

## **Soumettre une Pull Request**

1. **Poussez votre branche** sur votre fork :
   ```bash
   git push origin feature/nom-de-la-branche
   ```

2. **Créer une Pull Request** sur GitHub :
   - Allez dans l’onglet **Pull Requests** de votre fork.
   - Cliquez sur **New Pull Request**.
   - Assurez-vous de comparer votre branche à `develop` ou `main`.

3. **Décrivez votre PR** en suivant ce modèle :
   ```markdown
   ## Description
   [Décrivez brièvement vos modifications.]

   ## Issue associée
   Fixes #[NUMÉRO_DE_L_ISSUE]

   ## Changements
   - [Point 1 des modifications]
   - [Point 2 des modifications]

   ## Checklist
   - [ ] Les tests passent localement.
   - [ ] La documentation a été mise à jour.
   - [ ] Cette PR corrige l’issue associée.
   ```

4. **Répondez aux commentaires** :
   Les mainteneurs pourraient demander des modifications. Soyez réactif pour améliorer votre PR.

---

## **Code de Conduite**
En contribuant, vous acceptez de respecter notre [Code of Conduct](CODE_OF_CONDUCT.md).

---

## **Nous contacter**
Si vous avez des questions ou des suggestions, ouvrez une issue ou contactez un mainteneur directement via [email/contact GitHub].

---

### **Checklist pour les contributeurs**
Avant de soumettre une Pull Request :
- [ ] J’ai créé une branche descriptive.
- [ ] J’ai testé localement mes modifications.
- [ ] J’ai mis à jour la documentation si nécessaire.
- [ ] J’ai vérifié que les commits sont signés.

---