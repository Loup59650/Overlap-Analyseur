# Overlap-Analyseur

Overlap-Analyseur est un outil d'analyse financière développé en Python, conçu pour mesurer et optimiser la véritable diversification d'un portefeuille boursier. À l'origine, j'ai développé ce projet pour m'aider personnellement dans la constitution de mon propre portefeuille d'investissement, afin d'y voir plus clair dans mes allocations réelles. En effet, de nombreux investisseurs accumulent différents ETF, comme le MSCI World et le S&P 500, en pensant diversifier leurs actifs, sans réaliser qu'ils achètent souvent massivement les mêmes entreprises sous-jacentes. Ce projet résout ce problème de "fausse diversification" en traitant les données réelles de composition des fonds (holdings) grâce à la librairie Pandas.

Le script croise ces bases de données pour identifier les actions en commun, calculer le pourcentage exact de chevauchement (overlap) et mettre en évidence le risque de concentration. En prenant en compte l'allocation personnalisée de l'investisseur, l'outil détermine le poids réel et final de chaque action (comme Apple ou Microsoft) au sein du portefeuille global. 

Note méthodologique : Pour les ETF éligibles au PEA à réplication synthétique, l'algorithme utilise les proxys à réplication physique correspondants afin d'analyser l'exposition économique réelle
