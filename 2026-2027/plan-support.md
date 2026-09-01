# EFREI - M1 UX Design - Développement Web
## Plan du support de cours 2026-2027 (proposition de mise à jour)

Ce document décrit la structure cible du support de cours pour l'année 2026-2027, en évolution du support 2025-2026. Les mentions (inchangé), (actualisé), (refonte) et (nouveau) indiquent le travail à prévoir section par section.

---

### 1. Le Web et Internet (inchangé, ajustements mineurs)
- 1.1 Internet : c'est quoi exactement ? (TCP/IP, IP, DNS)
- 1.2 HTTP et les requêtes (méthodes, codes de réponse, HTTPS)
- 1.3 Le modèle client / serveur (navigateurs et moteurs de rendu)
- 1.4 L'hébergement web
- 1.5 Open source vs propriétaire

### 2. Les 3 domaines du Web (inchangé)
- 2.1 Vue d'ensemble
- 2.2 Le front-end
- 2.3 Le back-end
- 2.4 L'infrastructure

### 3. Les langages du Web (actualisé)
- 3.1 HTML, CSS et JavaScript : les trois piliers du front-end
- 3.2 HTML - un langage de balisage
- 3.3 CSS - les feuilles de style
- 3.4 JavaScript - comprendre et spécifier, sans écrire (actualisé)
  - Périmètre explicitement borné : reconnaître ce qui nécessite du JS, savoir le spécifier dans une spec, en mesurer le coût. Aucune écriture de code JS dans ce cours.

### 4. Vos outils : VS Code, navigateurs et DevTools (actualisé)
- 4.1 VS Code - installation, extensions, Emmet, raccourcis
- 4.2 Tester dans les navigateurs et ouvrir les DevTools
  - Retirer les références spécifiques à la promo 2025-2026 ("ce que vous avez vécu en cours") au profit d'un cas générique Safari vs Chrome.

### 5. HTML - Structure et sémantique (actualisé)
- 5.1 Structure d'une page HTML
- 5.2 La sémantique HTML : pourquoi les balises ont un sens
- 5.3 La responsivité (breakpoints, media queries, viewport)
  - Ajouter un encadré d'ouverture sur les container queries (penser responsive par composant).
- 5.4 Organisation des fichiers et chemins relatifs
- 5.5 Les liens
- 5.6 Les pièges des espaces et caractères
- 5.7 Les images (formats, alt, object-fit, background-image, performance)
  - Ajouter loading="lazy" dans la partie performance.
- 5.8 (nouveau) Les composants natifs interactifs : details / summary
  - L'accordéon sans une ligne de JS, accessible par défaut. Prépare le projet fil rouge.

### 6. CSS - Style et mise en page (refonte de la partie layout)
- 6.1 Le box model (inchangé)
- 6.2 Display : block, inline, inline-block (inchangé)
- 6.3 (nouveau) Flexbox - l'auto layout du web
  - Miroir systématique avec Figma : direction, gap, justify/align, hug/fill.
  - Patterns : header logo + navigation, rangée de cartes, centrage vertical.
- 6.4 (nouveau) Grid - la grille native
  - Grilles de cartes responsives (repeat, minmax, auto-fit), zones nommées.
  - Miroir avec les grilles Figma.
- 6.5 Positionnement : sticky, absolute, z-index (recentré)
  - float, vertical-align et line-height ne sont plus enseignés comme techniques de mise en page : ils passent dans un encadré "code hérité que vous croiserez en audit".
  - Le tableau récapitulatif "quelle technique pour quel besoin" est réécrit avec flexbox et grid en premières réponses.
- 6.6 Les sélecteurs CSS (inchangé, ajouter un mot sur :has() en ouverture)
- 6.7 Variables CSS et design tokens (actualisé)
  - Ajouter le mode sombre avec prefers-color-scheme : le cas d'usage roi des variables, réutilisé dans le projet fil rouge.
- 6.8 Transitions et animations (actualisé)
  - Ajouter prefers-reduced-motion : une décision de design, pas de code.
- 6.9 (nouveau) De l'interactivité sans JavaScript
  - details / summary (rappel), scroll-snap pour les galeries, :target, sticky.
  - Message clé : le CSS moderne couvre une grande partie de ce qui exigeait du JS il y a cinq ans.
- 6.10 Bonnes pratiques : BEM, organisation d'un fichier CSS, nommage (inchangé)
- 6.11 Exemple complet (actualisé)
  - L'exemple portfolio est remplacé par une mini landing page annotée, cohérente avec le projet fil rouge.

### 7. (nouveau) Web responsable : accessibilité et éco-conception
- 7.1 L'accessibilité, une compétence coeur du designer UX
  - Enjeux humains (15 % de la population) et cadre légal : European Accessibility Act (applicable depuis juin 2025), RGAA 4.1.2 en vigueur, RGAA 5 attendu fin 2026, sanctions jusqu'à 50 000 euros.
  - Les gestes concrets du designer : contrastes, focus visible, alt, labels, hiérarchie de titres, tailles de cibles tactiles, navigation clavier.
- 7.2 L'éco-conception : concevoir sobre
  - Le RGESN v2 (78 critères, 9 familles) et ce qui relève du design : fonctionnalités superflues, autoplay, densité, poids des médias, parcours courts.
  - Lien direct avec la performance (les images pèsent 60 à 70 % d'une page).
- 7.3 Auditer un site : le protocole complet
  - Absorbe et étend l'ancienne section 9 : inspection DevTools, test mobile, navigation clavier, contrastes, Lighthouse, EcoIndex.
  - Grille d'audit prête à l'emploi (celle utilisée en atelier et pour le rapport individuel).

### 8. Projet fil rouge - Landing page et mini design system (nouveau, remplace le CV)
- 8.1 Le brief : inventer un produit ou service fictif, en binôme
- 8.2 Les livrables : une landing page + une page styleguide (tokens et composants avec leurs états)
- 8.3 Les contraintes techniques imposées
  - HTML sémantique, layout flexbox/grid, responsive mobile-first, variables CSS, un accordéon details/summary, mode sombre prefers-color-scheme, zéro JavaScript.
- 8.4 Étapes guidées (alignées sur les ateliers des séances 2 à 4)
- 8.5 Le barème détaillé
- 8.6 Pour aller plus loin (scroll-snap, animations, déploiement GitHub Pages)

### 9. L'IA : vibe coding et vibe design (refonte)
- 9.1 L'émergence du vibe coding (conservé, vieillit bien)
- 9.2 Le paysage des outils, par usage plutôt que par produit (refonte)
  - Idéation 0-to-1, prototype testable, assistance au code, génération de composants.
  - Tableau d'outils daté "à jour en septembre 2026" : Stitch (refonte mars 2026 : canevas infini, agent de design, DESIGN.md, MCP), Figma Make, Claude Code, Cursor, Lovable, Bolt, v0. Retirer les mentions de modes produits obsolètes.
- 9.3 Ce que ça change pour le designer UX (conservé)
- 9.4 Les limites du code généré et le rôle du designer (conservé tel quel : accessibilité, sémantique, cohérence, performance)
- 9.5 Se préparer : prompter, auditer, comprendre sans écrire (conservé)

### 10. Faciliter le travail de vos développeurs (quasi inchangé)
- 10.1 Nommer de façon cohérente (Figma vers BEM)
- 10.2 Spécifier tous les états d'un composant
- 10.3 Penser responsive dès la maquette
- 10.4 Exporter proprement les assets
- 10.5 Fournir les alt texts dans les specs
- 10.6 Communiquer avec le bon vocabulaire

### Bibliographie et ressources (actualisé)
- Documentation de référence (MDN, web.dev)
- Apprendre HTML et CSS
- Accessibilité (renforcé : RGAA, design.numerique.gouv.fr, WebAIM)
- (nouveau) Éco-conception : RGESN, ecoresponsable.numerique.gouv.fr, EcoIndex, GR491
- Outils IA (tableau daté)
- Assets et outils gratuits

### Récapitulatif - ce que vous devez retenir (actualisé)
- Ajouter les acquis flexbox/grid, accessibilité et éco-conception à la liste des compétences finales.

---

## Mises à jour transverses du support
- Remplacer toutes les mentions "2025/2026" (topbar, meta description, titre, nom du fichier PDF) par "2026/2027".
- Regénérer le PDF après refonte.
- Le support HTML lui-même doit être exemplaire vis-à-vis du chapitre 7 (contrastes, focus visible, poids raisonnable) : il sert de démonstration.
