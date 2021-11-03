# JokeR
  <p align="center">
  <img src="../img/Joker.png" width="120" height="142">
  </p>

[Accueil](index) | Projet | [Publications](publications) | [Partenaires](partenaires) | [Nous contacter](contact) | [Outils](outils) | [<img src="../img/drapeau EN.png" width="20">](https://motsmachines.github.io/joker/EN/project)
<br>
  <h1 align="center"><a href="https://motsmachines.github.io/joker/EN">CLEF Workshop JOKER</a>:</h1>
  <h2 align="center">Traduction automatique des jeux de mots et de l'humour
</h2>

  <h3>Thèmes et objectifs</h3>
  
L'objectif est de fédérer la communauté scientifique intéressée par la localisation automatique de l'humour et des jeux de mots.  Le projet JokeR aborde la question de l'identité européenne à travers l'étude de l'humour dans une perspective interculturelle. L'objectif principal du projet JokeR est d'étudier les stratégies de localisation de l'humour et des jeux de mots et de créer un corpus parallèle multilingue, annoté selon ces stratégies, ouvert et librement disponible, ainsi que de développer des outils d'évaluation.

  <h3>Motivation & Pertinence par rapport à CLEF & Importance pour le champ d'étude</h3>

  La communication interculturelle repose largement sur la traduction. L'humour reste de loin l'un de ses aspects les plus complexes; pour comprendre l'humour, il faut souvent saisir les références culturelles implicites et/ou relever les doubles sens, ce qui pose bien sûr la question de l'(in)traductibilité de l'humour. Les jeux de mots constituent une source ordinaire d'humour et les romanciers, les poètes et les dramaturges les utilisent. Ont les trouve également dans les titres, les gros titres, les toponymes, les anthroponymes, les noms d'organisations et la publicité car ils attirent l'attention et présentent des qualités mnémotechniques, ludiques, subversives, etc. La traduction de l'humour et des jeux de mots est donc très valorisée. La traduction moderne s'appuie énormément sur les outils numériques, pourtant peu de travaux de recherche ont étudié l'automatisation de la traduction de l'humour et des calembours ou la création d'un corpus de l'humour. À notre connaissance, il n'existe pas de corpus parallèle.

  Le **corpus parallèle multilingue** issu des résultats de l'atelier JokeR constituera un pas en avant dans l'automatisation de la localisation de l'humour et permettra d'affiner et d'évaluer les modèles de traduction automatique. Il existe encore peu de corpus d'humour **monolingues** ; par exemple, les ensembles de données créés lors de l'atelier international sur l'évaluation sémantique SemEval <a href="#note1">[1]-[3]</a> : #HashtagWars : Learning a Sense of Humor (2017), Detection and Interpretation of English Puns (2017), Assessing Humor in Edited News Headlines (2020), HaHackathon : Detecting and Rating Humor and Offense (2021). Mihalcea et Strapparava <a href="#note1">[4]</a> ont permis de collecter 16 000 phrases humoristiques et un nombre égal d'échantillons négatifs à partir de titres de nouvelles, de proverbes, du British National Corpus et du jeu de données Open Mind Common Sense, tandis qu'un autre jeu de données contient 2 400 jeux de mots et non-jeu de mots, issus des informations, de Yahoo!Answers et de proverbes <a href="#note1">[5]</a>, <a href="#note2">[6]</a>. La plupart des ensembles de données sont en anglais ; on trouve quelques exceptions en italien <a href="#note2">[7]</a>, en russe <a href="#note2">[8]</a>, <a href="#note2">[9]</a>, et en espagnol <a href="#note2">[10]</a>.

  <h3>Domaine d'application</h3>

  Les données multilingues et les métriques résultant de l'atelier JokeR constitueront un pas en avant dans l'automatisation de la localisation de l'humour. Elles permettront d'entraîner et d'évaluer les modèles de traduction automatique. Ce corpus pourrait également être utile aux étudiants en traduction. 

  <h3>Mise en place de l'évaluation, mesures et tâches pilotes</h3>

  L'objectif de l'atelier JokeR est de réunir des traducteurs et des ingénieurs en informatique pour travailler sur un modèle d'évaluation du langage créatif. Tous les types de contributions seront les bienvenus :
  - Articles de recherche et articles de synthèse
  - Articles d'opinion, de discussion et de démonstration
  - Résumés détaillés d'articles publiés

  <h3>Principaux objectifs</h3>

**Objectif n°1**: Classer et expliquer une construction de calembour donnée dans un nom propre ou un néologisme. La classification sera évaluée en fonction de sa précision, tandis que l'explication sera comparée à l'étalon de référence (correspondance exacte).

**Objectif n°2**: Traduire un jeu de mots donné à partir d'un nom propre ou d'un néologisme de l'anglais vers le français.

**Objectif n°3**: Traduire un calembour donné de l'anglais vers le français.

Pour les tâches 2 et 3, il est nécessaire de concevoir des outils pour évaluer la qualité de la traduction. Traditionnellement, la qualité de la traduction automatique est mesurée par la métrique BLEU (Bilingual Evaluation Understudy), qui calcule le chevauchement de vocabulaire entre la traduction candidate et la traduction de référence <a href="#note2">[11]</a>. Cependant, aucune métrique basée sur le chevauchement de vocabulaire ne peut s'appliquer à l'évaluation d'une traduction en langage créatif. Ainsi, dans un premier temps, nous opterons pour un questionnaire à remplir par les annotateurs (" le jeu de mots est-il présent dans la traduction ? ", " le champ sémantique est-il préservé dans la traduction ? " etc...). Puis, à l'issue de l'atelier, nous étudierons l'automatisation des métriques choisies.  

<h3>La durée prévue de l'atelier lors de la conférence est d'une demi-journée :</h3>

Discours d'ouverture 15 min
  - Orateur invité 1 h
  - Présentations des participants 15 mins + 5 mins pour les questions
  - Discours de clôture 15 mins

<p>
<a href="./JOKER_CLEF_2021.pdf"><h3>Campagne d'évalutation CLEF (pdf en anglais)</h3></a>
</p>  

<h3 id="note1">Références:</h3>
  <p>
<p>[1]	‘SemEval-2021 Tasks’, SemEval-2021. https://semeval.github.io/SemEval2021/tasks.html (accessed Mar. 02, 2021).</p>
<p>[2]	‘Tasks < SemEval-2017’. https://alt.qcri.org/semeval2017/index.php?id=tasks (accessed Mar. 02, 2021).</p>
<p>[3]	‘Tasks < SemEval-2020’. https://alt.qcri.org/semeval2020/index.php?id=tasks (accessed Mar. 02, 2021).</p>
<p>[4]	R. Mihalcea and C. Strapparava, ‘Making Computers Laugh: Investigations in Automatic Humor Recognition’, in Proceedings of Human Language Technology Conference and Conference on Empirical Methods in Natural Language Processing, Vancouver, British Columbia, Canada, Oct. 2005, pp. 531–538. Accessed: Mar. 02, 2021. [Online]. Available: https://www.aclweb.org/anthology/H05-1067</p>
<p>[5]	A. Cattle and X. Ma, ‘Recognizing Humour using Word Associations and Humour Anchor Extraction’, in Proceedings of the 27th International Conference on Computational Linguistics, Santa Fe, New Mexico, USA, Aug. 2018, pp. 1849–1858. Accessed: Mar. 02, 2021. [Online]. Available: https://www.aclweb.org/anthology/C18-1157</p>
<p id="note2">[6]	D. Yang, A. Lavie, C. Dyer, and E. Hovy, ‘Humor Recognition and Humor Anchor Extraction’, in Proceedings of the 2015 Conference on Empirical Methods in Natural Language Processing, Lisbon, Portugal, Sep. 2015, pp. 2367–2376. doi: 10.18653/v1/D15-1284.</p>
<p>[7]	A. Reyes, D. Buscaldi, and P. Rosso, ‘An Analysis of the Impact of Ambiguity on Automatic Humour Recognition’, in Text, Speech and Dialogue, Berlin, Heidelberg, 2009, pp. 162–169. doi: 10.1007/978-3-642-04208-9_25.</p>
<p>[8]	V. Blinov, V. Bolotova-Baranova, and P. Braslavski, ‘Large Dataset and Language Model Fun-Tuning for Humor Recognition’, in Proceedings of the 57th Annual Meeting of the Association for Computational Linguistics, Florence, Italy, 2019, pp. 4027–4032. doi: 10.18653/v1/P19-1394.</p>
<p>[9]	A. Ermilov, N. Murashkina, V. Goryacheva, and P. Braslavski, ‘Stierlitz Meets SVM: Humor Detection in Russian’, in Artificial Intelligence and Natural Language, Cham, 2018, pp. 178–184. doi: 10.1007/978-3-030-01204-5_17.</p>
<p>[10]	S. Castro, L. Chiruzzo, A. Rosá, D. Garat, and G. Moncecchi, ‘A Crowd-Annotated Spanish Corpus for Humor Analysis’, in Proceedings of the Sixth International Workshop on Natural Language Processing for Social Media, Melbourne, Australia, Jul. 2018, pp. 7–11. doi: 10.18653/v1/W18-3502.</p>
<p>[11]	K. Papineni, S. Roukos, T. Ward, and W.-J. Zhu, ‘BLEU: a method for automatic evaluation of machine translation’, in Proceedings of the 40th annual meeting on association for computational linguistics, 2002, pp. 311–318.<p/>
  </p>


<p>
<em>Ce projet a bénéficié d'une aide de l'état gérée par l'Agence Nationale de la Recherche au titre du programme « Investissements d'avenir » portant la Référence ANR-19-GURE-0001</em>
</p>
<p>
<em>JokeR est labellisé par la Maison des Sciences de l'Homme en Bretagne</em>
</p>
<div align="center">
  <a href="https://www.mshb.fr"><img src="../img/MSHB.jpg" height="120"></a>
  <a href="https://sea-eu.org/?lang=fr"><img src="../img/SEA-EU.png" height="120"></a>
  <a href="https://www.gouvernement.fr/le-programme-d-investissements-d-avenir"><img src="../img/Investissement avenir.jpeg" height="120"></a>
</div>
<br />
<div align="center">
  <a href="https://clef2022.clef-initiative.eu/index.php"><img src="../img/CLEF2022.png" height="90"></a> 
</div>
