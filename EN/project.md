# JokeR
  <p align="center">
  <img src="../img/Joker.png" width="120" height="142">
  </p>

[Home](index) | CLEF | [Publications](publications) | [Partners](partners) | [Contest](contest) | [Contact Us](contact) | [Tools](tools)
<br>
  <h1 align="center">CLEF Workshop:</h1>
  <h2 align="center">Automatic Pun and Humour Translation</h2>

## Call for Participation 

### Context
Humour remains one of the most difficult aspects of intercultural communication: understanding humour often requires understanding implicit cultural references and/or double meanings, and this raises the question of its (un)translatability. Wordplay is a common source of humour due to its attention-getting and subversive character. The translation of humour and wordplay is therefore in high demand. Modern translation depends heavily on technological aids, yet few works have treated the automation of humour and wordplay translation, or the creation of humour corpora. The goal of the JOKER workshop is to bring together translators and computer scientists to work on an evaluation framework for wordplay, including data and metric development, and to foster work on automatic methods for wordplay translation.
### Tasks
We invite you to submit both automatic and manual runs! Manual intervention should be reported.
* Task 1: Сlassify and explain instances of wordplay.
* Task 2: Translate single words containing wordplay.
* Task 3: Translate entire phrases containing wordplay.
* Unshared task: We welcome any other type of submission that uses our data as an open task.

### Deadlines
* Run submission: 22 April 2022 
* Results available: 6 May 2022
* Draft paper submission: 27 May 2022
* Camera-ready submission: 1 July 2022
* CLEF conference: 5–8 September 2022

## Access
Sign up at the CLEF website (https://clef2022-labs-registration.dei.unipd.it/). All team members should join the JOKER mailing list (https://groups.google.com/u/4/g/joker-project). After registration, you will receive an email with information on how to get access to the data.

The data is split into 3 folders corresponding to the shared tasks. Each task folder is further split in train data and test data. 

Meta-data will be available as the participants' results will be published.

### Result submission:
Participants should put their run results into the folder Documents created for their user and **submit them by email** to *contact@joker-project.com*.

The email subject has to be in the format **\[CLEF TASK \<NUMBER\>\] TEAM_ID**. 

Runs should be submitted as a <ins>ZIP folder of the corresponding JSON files</ins>. Manual runs are allowed to be submitted in a CSV format. 

A confirmation email will be sent within 2 days after the submission deadline. 

## Task 1: Сlassify and explain instances of wordplay.

**Train data format:**
List of classified wordplay instances in a **JSON format** or a CSV file (for manual runs) with the following fields:
* `ID`: a unique wordplay identifier 
* `WORDPLAY`: wordplay text
* `TARGET_WORD`: word(s) 
* `DISAMBIGUATION`: explanation of the wordplay
* `HORIZONTAL/VERTICAL`: co-presence of source and target of the wordplay. In **horizontal** wordplay, both the source and the target of the wordplay are given (ex. 1: “They’re called <ins>lessons</ins> because they <ins>lessen</ins> from day to day”); in **vertical** wordplay, source and target are collapsed in a single occurrence (ex. 2: “How do you make a <ins>cat drink</ins>? Easy: put it in a liquidizer”)
* `MANIPULATION_TYPE`:  **Identity** (source and target are formally identical, as in ex. 2 above); **Similarity** (as in ex. 1 above: source and target are not perfectly identical, but the resemblance is obvious); **Permutation** (the textual material is given a new order, as in anagrams or spoonerism. Ex. 3: “Dormitory = dirty room”); **Abbreviation** (an ad-hoc category for textual material where the initials form another meaning, as in acrostics or “funny” acronyms. Ex. 4: “BRAINS: Biobehavioral Research Awards for Innovative New Scientists”)
* `MANIPULATION_LEVEL`: most wordplay involves some kind of phonological manipulation – that’s why **Sound** will be the default category. Examples 1 and 2 involve a clear sound similarity (ex. 1) or identity (ex. 2). Only if this category cannot be applied to the wordplay should you look for another level of manipulation.  First consider whether the manipulation involves **Writing** (as in ex. 3 and 4). If neither **Sound** nor **Writing** are manipulated, specify the level of manipulation as **Other**. This level of manipulation may arise, for instance, in chiasmuses (ex. 5: “We shape our buildings, and afterwards our buildings shape us”).	
* `CULTURAL_REFERENCE`:  this is a binary (**True/False**) category. In order to understand some instances of wordplay, one has to be aware of some extra-linguistic factors	
* `CONVENTIONAL_FORM`: this is a binary (**True/False**) category, e.g. *Tom Swifty* (wellerism), *Monsieur et Madame… ont un fils* 
* `OFFENSIVE` (not evaluated category): some wordplay instances are marked as offensive. 

*Example:*

```
[{"ID":"noun_1063","WORDPLAY":"Elimentaler","TARGET_WORD":"Elimentaler","DISAMBIGUATION":"Emmental (cheese) + Eliminator","HORIZONTAL\/VERTICAL":"vertical","MANIPULATION_TYPE":"Similarity","MANIPULATION_LEVEL":"Sound","CULTURAL_REFERENCE":false,"CONVENTIONAL_FORM":false,"OFFENSIVE":null},{"ID":"pun_341","WORDPLAY":"Geologists can be sedimental about their work.","TARGET_WORD":"sedimental","DISAMBIGUATION":"sentimental\/sediment","HORIZONTAL\/VERTICAL":"vertical","MANIPULATION_TYPE":"Similarity","MANIPULATION_LEVEL":"Sound","CULTURAL_REFERENCE":false,"CONVENTIONAL_FORM":false,"OFFENSIVE":null}]
```

**Test data input format:** 
List of wordplay instances to classify in a **JSON format** or a CSV file (for manual runs) with the following fields:
* `ID`: a unique wordplay identifier 
* `WORDPLAY`: wordplay text

*Input example:*

```
[{"ID":"noun_1","WORDPLAY":"Ambipom"},{"ID":"het_1011","WORDPLAY":"These are my parents, said Einstein relatively"}]
```

**Test data output format:** 

List of wordplay instances to be classified in a **JSON format** or a CSV file (for manual runs) with the following fields:
* `RUN_ID`: Run ID starting with **team_id_** (as registered at the CLEF website)
* `MANUAL`: Whether the run is manual {0,1}
* `ID`: a unique wordplay identifier from the input file 
* `WORDPLAY`: wordplay text
* `TARGET_WORD`: word(s) 
* `DISAMBIGUATION`: explanation of the wordplay
* `HORIZONTAL/VERTICAL`: co-presence of source and target of the wordplay (**horizontal/vertical**)
* `MANIPULATION_TYPE`:  **Identity/Similarity/Permutation/Abbreviation** 
* `MANIPULATION_LEVEL`: **Sound/Writing/Other**. 
* `CULTURAL_REFERENCE`:  this is a binary (**True/False**) category. In order to understand some instances of wordplay, one has to be aware of some extra-linguistic factors	
* `CONVENTIONAL_FORM`: this is a binary (**True/False**) category, e.g. *Tom Swifty* (wellerism), *Monsieur et Madame… ont un fils* 
* `OFFENSIVE` (not evaluated category): some wordplay instances are marked as offensive. 

*Output example*:

```
[{"RUN_ID":"RT","MANUAL":1,"ID":"noun_1063","WORDPLAY":"Elimentaler","TARGET_WORD":"Elimentaler","DISAMBIGUATION":"Emmental (cheese) + Eliminator","HORIZONTAL\/VERTICAL":"vertical","MANIPULATION_TYPE":"Similarity","MANIPULATION_LEVEL":"Sound","CULTURAL_REFERENCE":false,"CONVENTIONAL_FORM":false,"OFFENSIVE":null},{"RUN_ID":"RT","MANUAL":1,"ID":"pun_341","WORDPLAY":"Geologists can be sedimental about their work.","TARGET_WORD":"sedimental","DISAMBIGUATION":"sentimental\/sediment","HORIZONTAL\/VERTICAL":"vertical","MANIPULATION_TYPE":"Similarity","MANIPULATION_LEVEL":"Sound","CULTURAL_REFERENCE":false,"CONVENTIONAL_FORM":false,"OFFENSIVE":null}]
```
#### Evaluation
Pilot Task 1 includes both classification and interpretation components. Classification performance will be evaluated with respect to accuracy, while interpretation performance will be evaluated semi-manually.

#### Result submission:
Participants should put their run results into the folder Documents created for their user and **submit them by email** to *contact@joker-project.com*.

The email subject has to be in the format **\[CLEF TASK 1] TEAM_ID**. 

### Terms of Use

By downloading and using JOKER data, you agree to the terms of use. Any use of the data for any purpose other than academic research, would be in violation of the intended use of these data. 

Therefore, by downloading and using these data you give the following assurances with respect to the JOKER data:
1. You will not use nor permit others to use the data in the JOKER datasets in any way except for classes and academic research.
2. You will not at any time disclose, give, or transmit (in any manner or form or for any purpose) the data (or any portion thereof) to any location or person, including but not limiting to making the data available on the Internet, and copying the data onto any cloud-based storage system.
3. You will not release nor permit others to release the dataset or any part of it to any person. 

In case of violation of the conditions for access to the data for scientific purposes, this access may be withdrawn from the research entity and/or from the researcher. The research entity may also be liable to pay compensation for damages for third parties or asked to take disciplinary action against the offending researcher. 




[JOKER@CLEF presentation (pdf)](./JOKER_CLEF_2021.pdf)

[1-st Call for Participation (pdf)](../1st Call JOKER 2022.pdf)

  
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
