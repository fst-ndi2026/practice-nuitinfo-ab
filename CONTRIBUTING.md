# Contribuer / المساهمة

Règle d'or : **personne ne pousse directement sur `main`**. Tout passe par une branche et une Pull Request.
القاعدة الذهبية: **لا أحد يدفع مباشرة إلى `main`**. كل تغيير يمرّ عبر فرع ثم Pull Request.

## 1. Avant de commencer une tâche / قبل بدء أي مهمة

```bash
git switch main
git pull
git switch -c feat/nom-court-de-la-tache
```

Préfixes de branche / بادئات الفروع :

| Préfixe  | Usage / الاستعمال                    |
| -------- | ------------------------------------ |
| `feat/`  | nouvelle fonctionnalité / ميزة جديدة |
| `fix/`   | correction de bug / إصلاح خطأ        |
| `style/` | design, CSS / تصميم                  |
| `chore/` | config, outils / إعدادات وأدوات      |
| `docs/`  | documentation / توثيق                |

Exemple : `feat/page-accueil`, `fix/bouton-contact`.

## 2. Pendant le travail / أثناء العمل

- Commits petits et fréquents, message clair : `git commit -m "Ajoute le formulaire de contact"`.
- Avant de pousser / قبل الدفع :

```bash
npm run format
npm run lint
npm run build
```

## 3. Ouvrir une Pull Request / فتح Pull Request

```bash
git push -u origin feat/nom-court-de-la-tache
```

Puis sur GitHub : **Compare & pull request** → remplir le modèle → demander une relecture.
ثم على GitHub: اضغط **Compare & pull request** واملأ القالب واطلب مراجعة من زميل.

- La CI (format + lint + build) doit être ✅.
- Vercel publie automatiquement un **lien de prévisualisation** dans la PR : testez-le.
- **1 approbation** d'un coéquipier est nécessaire avant le merge.
- Merge avec **Squash and merge**, puis supprimer la branche.

## 4. En cas de conflit / عند حدوث تعارض

```bash
git switch main
git pull
git switch feat/ma-branche
git merge main
# résoudre les conflits dans VS Code, puis :
git add .
git commit
git push
```

Bloqué ? Demandez de l'aide dans le groupe de l'équipe plutôt que de forcer (`--force`).
عالق؟ اطلب المساعدة من الفريق بدل استعمال `--force`.
