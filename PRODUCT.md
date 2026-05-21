# Product

## Register

product

## Users

Utilisateurs francophones qui veulent suivre objectifs, habitudes et journal personnel depuis leur téléphone, le soir ou tôt le matin — moments calmes. Public SaaS visé : individus exigeants sur l'esthétique, déjà familiers d'outils comme Things 3, Linear, Arc, Raycast. Ils n'utilisent pas Track pour gagner des points : ils l'utilisent pour reprendre la main sur leur temps.

Contexte d'usage : écran de téléphone tenu d'une main, souvent dans une pièce peu éclairée. Sessions courtes (30 s à 2 min) répétées, jamais des séances de 20 minutes.

## Product Purpose

Track est un compagnon discret pour suivre ce qui compte vraiment : objectifs long-terme, habitudes quotidiennes, et un journal léger. Pas un coach, pas un jeu : un outil qui rend la rigueur agréable et la consultation rapide.

Succès = l'utilisateur ouvre l'app sans y penser, fait sa saisie en moins de 30 secondes, et ressort sans avoir été distrait. Mesuré par la rétention silencieuse, pas par les notifications cliquées.

## Brand Personality

Sombre · cinématique · premium.

- **Voice** : posé, jamais enjoué. Phrases courtes. Pas d'exclamations, pas d'emojis dans l'UI.
- **Tone** : celui d'un éditeur de polices haut de gamme ou d'une revue cinéma — confiance tranquille, érudition légère.
- **Émotion visée** : la sensation d'ouvrir un carnet en cuir dans un bureau bien éclairé le soir, pas celle d'ouvrir une notification Duolingo.

## Anti-references

- **SaaS générique bleu/violet** : Stripe-clones, Linear-clones bleu électrique, dashboards Vercel-like. Track n'est pas un outil B2B.
- **Gamification visible** : confettis, badges, XP, streaks célébrés bruyamment, médailles. Les streaks peuvent exister mais doivent rester sobres.
- **Bootstrap / template flat** : grilles de cards identiques, ombres molles uniformes, icônes Heroicons par défaut.
- **Light mode joyeux** : tons crème/sable chaleureux, pastels, hand-drawn. Track est nocturne par design.
- **Dashboard data-viz** : graphiques élaborés en page d'accueil. Les chiffres servent la consultation, pas la démonstration.

## Design Principles

1. **Le produit s'efface.** L'utilisateur revient parce que l'app est silencieuse, pas parce qu'elle réclame son attention. Pas de notification dans l'UI, pas de prompt non sollicité.

2. **Cinéma, pas gaming.** La récompense vient de la matière (contraste, lumière, grain typographique), jamais d'une animation festive ou d'un badge. Quand on coche une habitude, c'est une transition élégante, pas un feu d'artifice.

3. **Une seule couleur qui parle.** Le dark est tinté, jamais pur noir. Tout est neutre sauf un accent unique utilisé avec parcimonie (≤10% des surfaces actives). L'accent gagne sa puissance par sa rareté.

4. **Le dark est intentionnel, pas un toggle.** Pas de switch light/dark proposé en V1. Le médium fait partie du produit ; le proposer en light l'affadirait.

5. **La typo porte la hiérarchie.** Pas d'ombres décoratives, pas de bordures épaisses colorées, pas de gradients. Échelle, poids et couleur font tout le travail.

## Accessibility & Inclusion

- **WCAG AAA** sur les contrastes texte (ratio ≥ 7:1 pour le corps, ≥ 4.5:1 pour les éléments graphiques larges).
- **Focus visibles partout** — bordure outline 2px en accent, pas de `outline: none` sans remplacement.
- **`prefers-reduced-motion`** respecté : toutes les transitions > 150ms se réduisent ou disparaissent.
- **Tap targets ≥ 44×44 px** (recommandation iOS HIG).
- **Pas de couleur seule** pour transmettre un état : toujours doubler avec icône, texte ou pattern.
