# UOI Games — Étude de marché & recommandation Triple A

Étude de marché complète menée pour un studio de jeu vidéo fictif (UOI Games) envisageant de lancer son premier jeu Triple A : analyse des tendances du marché (SWOT, PESTEL), segmentation de la clientèle à partir d'un catalogue de 440 000+ jeux, validation par questionnaire terrain (tests de corrélation), et recommandation finale de concept et d'écosystème.

Projet réalisé dans le cadre du parcours Business Intelligence Analyst (OpenClassrooms) — Aurélie Dupassieux, Data ESN.

## Notebook de synthèse

**[`UOI_Games_Synthese.ipynb`](UOI_Games_Synthese.ipynb)** condense l'ensemble de la démarche en un seul document exécutable : données → tendances marché → segmentation → validation terrain → recommandation finale, avec le code et les graphiques essentiels.

## Aller plus loin

Les 5 notebooks détaillés (un par phase du projet) sont disponibles dans [`notebooks_detailles/`](notebooks_detailles/) :

| Phase | Contenu |
|---|---|
| 1 | Nettoyage et exploration des 3 jeux de données sources |
| 2 | Tendances marché 2025-2026, matrice SWOT, analyse PESTEL |
| 3 | Segmentation chiffrée à partir du catalogue, conception du questionnaire |
| 4 | Tests de corrélation sur les réponses au questionnaire (Chi², V de Cramér, Spearman) |
| 5 | Recommandation finale : segment, concept de jeu, écosystème, prévision de ventes |

## Données

Le dossier `data/` contient les jeux de données nécessaires pour ré-exécuter le notebook de synthèse : ventes de jeux (1980-2020), ventes de consoles, réponses au questionnaire, et deux tableaux agrégés issus du catalogue de jeux. **Le catalogue complet (440 896 jeux, ~120 Mo une fois nettoyé) n'est pas inclus** pour garder ce dépôt léger — le notebook de synthèse s'appuie sur les agrégats déjà calculés (`genre_plateforme_agg.csv`, `esrb_par_genre_agg.csv`) ; le détail du traitement du catalogue complet est dans `notebooks_detailles/P10_Phase1_Nettoyage.ipynb`.

## Reproduire l'analyse

```bash
pip install pandas numpy matplotlib scipy pyxlsb jupyter
jupyter notebook UOI_Games_Synthese.ipynb
```
