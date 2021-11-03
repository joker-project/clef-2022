# JokeR
  <p align="center">
  <img src="../img/Joker.png" width="120" height="142">
  </p>

[Home](index) | Project | [Publications](publications) | [Partners](partners) | [Contact Us](contact) | [Tools](tools) | [<img src="../img/drapeau FR.png" width="20">](https://motsmachines.github.io/joker/FR/projet)
<br>
  <h1 align="center"><a href="https://motsmachines.github.io/joker/EN">CLEF Workshop JOKER</a>:</h1>
  <h2 align="center">Automatic Pun and Humour Translation</h2>

  <h3>Topics & Goals</h3>
  
  The goal is to unify the scientific community interested in automatic localization of humor and puns.  The JokeR project addresses the issue of European identity through the study of humor in a cross-cultural perspective. The main objective of the JokeR project is to study the strategies of localization of humor and puns and to create a multilingual parallel corpus, annotated according to these strategies, open and freely available, as well as evaluation metrics.

  <h3>Motivation & Relevance to CLEF & Significance for the field</h3> 

  Intercultural communication relies heavily on translation. Humor remains by far one of its most difficult aspects; to understand humor, one often has to grasp implicit cultural references and/or capture double meanings, which of course raises the question of the (in)translatability of humor. Puns are a common source of humor and are used by novelists, poets, and playwrights, as well as in titles, headlines, toponyms, anthroponyms, organizations, and advertising for their attention-getting or mnemonic, playful, subversive, etc. values. The translation of humor and puns is therefore in high demand. Modern translation is heavily aided by technological tools, yet few works have studied the automation of humor and puns translation and the creation of humor corpora. To the best of our knowledge, there does not exist any parallel corpus.

  The **multilingual parallel corpus** issued as the results of the JokeR workshop will be a step forward in the automatization of humour localization so as to train and evaluate machine translation models. Few **monolingual** humour corpora exist; for example, datasets created for the tasks of the International Workshop on Semantic Evaluation SemEval <a href="#note1">[1]–[3]</a>: #HashtagWars: Learning a Sense of Humor (2017), Detection and Interpretation of English Puns (2017), Assessing Humor in Edited News Headlines (2020), HaHackathon: Detecting and Rating Humor and Offense (2021). Mihalcea and Strapparava <a href="#note1">[4]</a> collected 16,000 humorous sentences and an equal number of negative samples from news titles, proverbs, British National Corpus, and the Open Mind Common Sense dataset, while another dataset contains 2,400 puns and not-puns from the news, Yahoo!Answers, and proverbs <a href="#note1">[5]</a>, <a href="#note2">[6]</a>. Most datasets are in English; few exceptions in Italian <a href="#note2">[7]</a>, Russian <a href="#note2">[8]</a>, <a href="#note2">[9]</a>, and Spanish <a href="#note2">[10]</a>.

  <h3>Application domain</h3>

  The multilingual data and metrics resulting from the JokeR workshop will be a step forward in the automation of humor localization in order to train and evaluate machine translation models. This corpus might also be useful for translation students. 

  <h3>Evaluation setup, metrics and pilot tasks</h3>

  The goal of the JokeR workshop is to bring together translators and computer scientists to work on an evaluation framework for creative langage. All types of contributions will be welcomed:
  - Research & survey papers
  - Position, discussion & demo papers
  - Extended abstracts of published papers

  <h3>Pilot tasks</h3>

**Pilot task 1**: Classify and explain a given punning construction in a proper noun or a neologism. The classification will be evaluated by the accuracy, while the explanation will be compared against the gold-standard (exact match).

**Pilot task 2**: Translate a given pun from a proper noun or a neologism from English into French

**Pilot task 3**: Translate a given punning phrase from English into French. 

For the tasks 2& 3, it is necessary to establish metrics for evaluating translation quality. Traditionally, machine translation quality is measured by the BLEU (Bilingual Evaluation Understudy) metric, which calculates vocabulary overlap between the candidate translation and the reference translation <a href="#note2">[11]</a>. However, no metric based on vocabulary overlap is applicable to evaluate creative language translation. First, we will opt for a questionnaire to be filled in by the annotators ("is the wordplay present in the translation?", "is the semantic field preserved in the translation?” etc.). At the end of the workshop, we will study the automation of the selected metrics. 

<h3>Expected length of the workshop at the conference is half-day:</h3>

Opening speech 15 min
  - Guest speaker 1 h
  - Presentations of the participants 15 mins + 5 min for questions
  - Closing speech 15 mins

<p>
  <a href="./JOKER_CLEF_2021.pdf"><h3>CLEF evaluation campaign (pdf)</h3></a>
</p>

<h3 id="note1">References:</h3>
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
<em>This project has received a government grant managed by the National Research Agency under the program "Investissements d'avenir" with the Reference ANR-19-GURE-0001</em>
</p>
<p>
<em>JokeR is supported by The Human Science Institute in Brittany (MSHB)</em>
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
