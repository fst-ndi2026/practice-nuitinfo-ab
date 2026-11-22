# NuitInfo Starter — Nuit de l'Info 2026

Projet de base de l'équipe pour la Nuit de l'Info 2026.
المشروع الأساسي للفريق في مسابقة Nuit de l'Info 2026.

🌐 **Production :** _à compléter après la connexion Vercel_

## Stack

| Outil                                          | Rôle / الدور                                     |
| ---------------------------------------------- | ------------------------------------------------ |
| [React 19](https://react.dev)                  | Interface utilisateur / واجهة المستخدم           |
| [TypeScript 6](https://www.typescriptlang.org) | JavaScript typé / جافاسكربت مع الأنواع           |
| [Vite 8](https://vite.dev)                     | Serveur de dev + build / خادم التطوير والبناء    |
| [Tailwind CSS 4](https://tailwindcss.com)      | Styles utilitaires / التنسيق                     |
| ESLint + Prettier                              | Qualité et formatage du code / جودة وتنسيق الكود |
| GitHub Actions                                 | CI : vérifie chaque PR / فحص تلقائي              |
| Vercel                                         | Déploiement automatique / النشر التلقائي         |

## Démarrage rapide / البدء السريع

Prérequis / المتطلبات : **Node.js 24+**, **npm**, **Git**, **VS Code**.

```bash
git clone <URL_DU_DEPOT>
cd <NOM_DU_DEPOT>
npm install
npm run dev
```

Puis ouvrir / ثم افتح : http://localhost:5173

À l'ouverture du projet, VS Code propose d'installer les extensions recommandées (Prettier, ESLint, Tailwind CSS IntelliSense) : acceptez.
عند فتح المشروع، يقترح VS Code تثبيت الإضافات الموصى بها: وافق.

## Commandes / الأوامر

| Commande               | Action                                             |
| ---------------------- | -------------------------------------------------- |
| `npm run dev`          | Serveur de développement avec rechargement à chaud |
| `npm run build`        | Vérifie TypeScript puis génère `dist/`             |
| `npm run preview`      | Sert le build de production en local               |
| `npm run lint`         | Analyse le code avec ESLint                        |
| `npm run format`       | Formate tout le code avec Prettier                 |
| `npm run format:check` | Vérifie le formatage (utilisé par la CI)           |

## Structure

```
├── .github/            CI + modèle de Pull Request
├── .vscode/            Réglages et extensions partagés
├── public/             Fichiers statiques servis tels quels
├── src/
│   ├── components/     Composants React réutilisables
│   ├── assets/         Images importées dans le code
│   ├── App.tsx         Composant racine
│   ├── main.tsx        Point d'entrée
│   └── index.css       Import Tailwind + styles globaux
├── index.html
└── vite.config.ts      Plugins React + Tailwind
```

## Travailler en équipe / العمل الجماعي

Voir **[CONTRIBUTING.md](CONTRIBUTING.md)** : une branche par tâche, Pull Request vers `main`, CI verte + 1 relecture avant merge.
راجع **[CONTRIBUTING.md](CONTRIBUTING.md)**: فرع لكل مهمة، ثم Pull Request إلى `main`.
