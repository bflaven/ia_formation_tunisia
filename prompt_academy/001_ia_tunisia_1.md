# 001_ia_tunisia_1.md

**Quelques adresses :**

- Mistral https://chat.mistral.ai/chat
- Claude https://claude.ai/new
- Perplexity https://www.perplexity.ai/
- Chatgpt (open AI) https://chatgpt.com/
- Gemini (Google) https://gemini.google.com/app




## USER STORY FORMATION

- **US : Assistance à l'écriture**

Nom	: Résumé

UserStory : En tant que journaliste, je souhaite, dans la même langue, avoir une proposition de draft d'un article depuis un contenu texte (article, édition, transcription...)	optimisé pour le référencement naturel.

Persona : JOURNALISTE



- **US : Résumé**

Nom	: Résumé

UserStory : En tant que journaliste, je souhaite, dans la même langue, avoir une proposition de résumé depuis un contenu texte (article, édition, transcription...)	

Persona : JOURNALISTE


## PROMPTS JOUR_1

**PROMPT : Générer un article**
```text
Écris un article pour le web à partir d’un texte que je te transmets. L’article fera 800 mots et sera optimisé pour le référencement naturel. Le chapô fera trois lignes maximum. L’article sera articulé en 7 paragraphes de 12 lignes chacun. Tu placeras 3 intertitres. Chaque intertitre ne dépassera pas 10 mots.

Voici le texte original : 

### Liverpool sacré champion d'Angleterre après sa victoire contre Tottenham
Sports. Grâce à sa large victoire 5-1 contre Tottenham dimanche, Liverpool a été sacré champion d'Angleterre. Cette fois, ils ont pu fêter le titre avec leurs supporters, contrairement à 2020, lorsque leur précédent sacre avait été éclipsé par la pandémie de Covid-19. Le joueur de Liverpool Mohamed Salah célèbre son quatrième but avec ses coéquipiers contre Tottenham, le 27 avril 2025, lors du Championnat d'Angleterre.
Liverpool a offert à ses supporters le sacre et la fête dont ils rêvaient, dimanche 27 avril à Anfield, avec une victoire enflammée contre Tottenham (5-1) synonyme de 20e titre en championnat d'Angleterre, le premier depuis 2020. Le Covid avait privé le peuple rouge d'une célébration méritée, il y a cinq ans, et il n'était pas question de gâcher la première "finale" de cette fin de saison, à domicile. Au coup de sifflet, les larmes des supporters se sont mêlés aux fumigènes et les joueurs ont dansé sur l'entêtant "Freed From Desire" de Gala, avant de se tenir, bras dessus bras dessous, devant le mythique Kop pour un très puissant "You'll Never Walk Alone". ###


```

**PROMPT : Générer 3 titres**

```text
Tu es un journaliste. Rédige trois titres convaincants et uniques pour un article en ligne sur le sujet donné. Assure-toi d'incorporer les meilleures pratiques SEO en incluant les mots-clés les plus courants et pertinents du contenu dans chaque titre. 


### Liverpool sacré champion d'Angleterre après sa victoire contre Tottenham
Sports. Grâce à sa large victoire 5-1 contre Tottenham dimanche, Liverpool a été sacré champion d'Angleterre. Cette fois, ils ont pu fêter le titre avec leurs supporters, contrairement à 2020, lorsque leur précédent sacre avait été éclipsé par la pandémie de Covid-19. Le joueur de Liverpool Mohamed Salah célèbre son quatrième but avec ses coéquipiers contre Tottenham, le 27 avril 2025, lors du Championnat d'Angleterre.
Liverpool a offert à ses supporters le sacre et la fête dont ils rêvaient, dimanche 27 avril à Anfield, avec une victoire enflammée contre Tottenham (5-1) synonyme de 20e titre en championnat d'Angleterre, le premier depuis 2020. Le Covid avait privé le peuple rouge d'une célébration méritée, il y a cinq ans, et il n'était pas question de gâcher la première "finale" de cette fin de saison, à domicile. Au coup de sifflet, les larmes des supporters se sont mêlés aux fumigènes et les joueurs ont dansé sur l'entêtant "Freed From Desire" de Gala, avant de se tenir, bras dessus bras dessous, devant le mythique Kop pour un très puissant "You'll Never Walk Alone". ###
```

**PROMPT : Générer 3 titres et introduire la variable français**

```text
Tu es un journaliste en francais. Rédige trois titres convaincants et uniques pour un article en ligne sur le sujet donné. Assure-toi d'incorporer les meilleures pratiques SEO en incluant les mots-clés les plus courants et pertinents du contenu dans chaque titre. 

Voici le texte original : 

### Liverpool sacré champion d'Angleterre après sa victoire contre Tottenham
Sports. Grâce à sa large victoire 5-1 contre Tottenham dimanche, Liverpool a été sacré champion d'Angleterre. Cette fois, ils ont pu fêter le titre avec leurs supporters, contrairement à 2020, lorsque leur précédent sacre avait été éclipsé par la pandémie de Covid-19. Le joueur de Liverpool Mohamed Salah célèbre son quatrième but avec ses coéquipiers contre Tottenham, le 27 avril 2025, lors du Championnat d'Angleterre.
Liverpool a offert à ses supporters le sacre et la fête dont ils rêvaient, dimanche 27 avril à Anfield, avec une victoire enflammée contre Tottenham (5-1) synonyme de 20e titre en championnat d'Angleterre, le premier depuis 2020. Le Covid avait privé le peuple rouge d'une célébration méritée, il y a cinq ans, et il n'était pas question de gâcher la première "finale" de cette fin de saison, à domicile. Au coup de sifflet, les larmes des supporters se sont mêlés aux fumigènes et les joueurs ont dansé sur l'entêtant "Freed From Desire" de Gala, avant de se tenir, bras dessus bras dessous, devant le mythique Kop pour un très puissant "You'll Never Walk Alone". ###
```

**PROMPT : Générer 3 titres et introduire la variable anglais**

```text
Tu es un journaliste en anglais. Rédige trois titres convaincants et uniques pour un article en ligne sur le sujet donné. Assure-toi d'incorporer les meilleures pratiques SEO en incluant les mots-clés les plus courants et pertinents du contenu dans chaque titre. 

Voici le texte original : 

### Liverpool sacré champion d'Angleterre après sa victoire contre Tottenham
Sports. Grâce à sa large victoire 5-1 contre Tottenham dimanche, Liverpool a été sacré champion d'Angleterre. Cette fois, ils ont pu fêter le titre avec leurs supporters, contrairement à 2020, lorsque leur précédent sacre avait été éclipsé par la pandémie de Covid-19. Le joueur de Liverpool Mohamed Salah célèbre son quatrième but avec ses coéquipiers contre Tottenham, le 27 avril 2025, lors du Championnat d'Angleterre.
Liverpool a offert à ses supporters le sacre et la fête dont ils rêvaient, dimanche 27 avril à Anfield, avec une victoire enflammée contre Tottenham (5-1) synonyme de 20e titre en championnat d'Angleterre, le premier depuis 2020. Le Covid avait privé le peuple rouge d'une célébration méritée, il y a cinq ans, et il n'était pas question de gâcher la première "finale" de cette fin de saison, à domicile. Au coup de sifflet, les larmes des supporters se sont mêlés aux fumigènes et les joueurs ont dansé sur l'entêtant "Freed From Desire" de Gala, avant de se tenir, bras dessus bras dessous, devant le mythique Kop pour un très puissant "You'll Never Walk Alone". ###
```

**PROMPT : Générer le résumé sans longueur spécifique**

``` text
Le résumé doit être dans la même langue que le texte original.
Il doit capturer les idées principales et les points clés du texte.
Le résumé ne doit pas inclure de phrases mot pour mot issues du texte original.


Voici le texte original : 

### Liverpool sacré champion d'Angleterre après sa victoire contre Tottenham
Sports. Grâce à sa large victoire 5-1 contre Tottenham dimanche, Liverpool a été sacré champion d'Angleterre. Cette fois, ils ont pu fêter le titre avec leurs supporters, contrairement à 2020, lorsque leur précédent sacre avait été éclipsé par la pandémie de Covid-19. Le joueur de Liverpool Mohamed Salah célèbre son quatrième but avec ses coéquipiers contre Tottenham, le 27 avril 2025, lors du Championnat d'Angleterre.
Liverpool a offert à ses supporters le sacre et la fête dont ils rêvaient, dimanche 27 avril à Anfield, avec une victoire enflammée contre Tottenham (5-1) synonyme de 20e titre en championnat d'Angleterre, le premier depuis 2020. Le Covid avait privé le peuple rouge d'une célébration méritée, il y a cinq ans, et il n'était pas question de gâcher la première "finale" de cette fin de saison, à domicile. Au coup de sifflet, les larmes des supporters se sont mêlés aux fumigènes et les joueurs ont dansé sur l'entêtant "Freed From Desire" de Gala, avant de se tenir, bras dessus bras dessous, devant le mythique Kop pour un très puissant "You'll Never Walk Alone". ###
```

**PROMPT : Faire 3 tweets avec des hashtags et des émojis**

```text
Tu es un community manager intelligent et compétent.
Rédige trois messages convaincants de 280 caractères chacun pour une publication en ligne en {langue} sur le sujet donné dans le contenu en {langue}.
Veille à intégrer les meilleures pratiques d'optimisation pour les réseaux sociaux (SMO) en incluant les mots-clés les plus courants du contenu.

Voici le texte original : 

### Liverpool sacré champion d'Angleterre après sa victoire contre Tottenham
Sports. Grâce à sa large victoire 5-1 contre Tottenham dimanche, Liverpool a été sacré champion d'Angleterre. Cette fois, ils ont pu fêter le titre avec leurs supporters, contrairement à 2020, lorsque leur précédent sacre avait été éclipsé par la pandémie de Covid-19. Le joueur de Liverpool Mohamed Salah célèbre son quatrième but avec ses coéquipiers contre Tottenham, le 27 avril 2025, lors du Championnat d'Angleterre.
Liverpool a offert à ses supporters le sacre et la fête dont ils rêvaient, dimanche 27 avril à Anfield, avec une victoire enflammée contre Tottenham (5-1) synonyme de 20e titre en championnat d'Angleterre, le premier depuis 2020. Le Covid avait privé le peuple rouge d'une célébration méritée, il y a cinq ans, et il n'était pas question de gâcher la première "finale" de cette fin de saison, à domicile. Au coup de sifflet, les larmes des supporters se sont mêlés aux fumigènes et les joueurs ont dansé sur l'entêtant "Freed From Desire" de Gala, avant de se tenir, bras dessus bras dessous, devant le mythique Kop pour un très puissant "You'll Never Walk Alone". ###
```

**PROMPT : Faire un resumé en 5 phrases**

```text
Produis un résumé du texte d'une longueur de 5 phrases.
Le résumé doit être dans la même langue que le texte original en '{language}'.
Il doit capturer les idées principales et les points clés du texte.
Le résumé ne doit pas inclure de phrases mot pour mot du texte original.

Voici le texte original : 

### Liverpool sacré champion d'Angleterre après sa victoire contre Tottenham
Sports. Grâce à sa large victoire 5-1 contre Tottenham dimanche, Liverpool a été sacré champion d'Angleterre. Cette fois, ils ont pu fêter le titre avec leurs supporters, contrairement à 2020, lorsque leur précédent sacre avait été éclipsé par la pandémie de Covid-19. Le joueur de Liverpool Mohamed Salah célèbre son quatrième but avec ses coéquipiers contre Tottenham, le 27 avril 2025, lors du Championnat d'Angleterre.
Liverpool a offert à ses supporters le sacre et la fête dont ils rêvaient, dimanche 27 avril à Anfield, avec une victoire enflammée contre Tottenham (5-1) synonyme de 20e titre en championnat d'Angleterre, le premier depuis 2020. Le Covid avait privé le peuple rouge d'une célébration méritée, il y a cinq ans, et il n'était pas question de gâcher la première "finale" de cette fin de saison, à domicile. Au coup de sifflet, les larmes des supporters se sont mêlés aux fumigènes et les joueurs ont dansé sur l'entêtant "Freed From Desire" de Gala, avant de se tenir, bras dessus bras dessous, devant le mythique Kop pour un très puissant "You'll Never Walk Alone". ###
```

## PROMPTS JOUR_2


**PROMPT :  Générer 3 titres depuis une URL (chatgpt)**

```text
Agis comme un journaliste d'un média radio international. Peux-tu me proposer trois titres différents pour cet article. Les titres devront être optimisés pour le référencement naturel et le plus accrocheur possible pour le lecteur. Voici l'URL de l'article : https://www.france24.com/fr/europe/20250429-panne-g%C3%A9ante-electricite-retour-%C3%A0-la-normale-en-espagne-et-au-portugal-trains

```

**PROMPT : Générer un resumé depuis une URL (chatgpt)**

```text
Peux-tu résumer cet article en 150 mots tu présenteras les principales informations sous forme de liste à puce et tu tâcheras d'écrire des phrases simples compréhensibles pour un enfant de 10 ans : : https://www.france24.com/fr/europe/20250429-panne-g%C3%A9ante-electricite-retour-%C3%A0-la-normale-en-espagne-et-au-portugal-trains
```


**PROMPT Changer la forme d'un article depuis une URL (chatgpt)**
```text
Change la forme de cet article sous forme de tableau avec trois colonnes : l'entreprise, le montant de l'amende et la date 

https://www.ledauphine.com/science-et-technologie/2021/11/11/google-amazon-apple-quelles-amendes-a-deja-infligees-l-ue-et-avec-quels-resultats
```

**PROMPT Faire des graphiques + tableur excel (esperance-de-vie-par-departements.csv) (chatgpt)**
```text
Agis comme un journaliste de radio grand public, lis avec attention les données de ce tableau, analyse ses données et propose 5 graphiques pour les illustrer et réalise ensuite ces différents graphiques dans les tons rouges.

```

**PROMPT : Introduire les variables language, contenu et un format de sortie. Depuis un {contenu} en {language} , générer 3 titres et 5 mots-clés en {language}**

```text
language = "français"
contenu = """
Liverpool sacré champion d'Angleterre après sa victoire contre Tottenham
Sports. Grâce à sa large victoire 5-1 contre Tottenham dimanche, Liverpool a été sacré champion d'Angleterre. Cette fois, ils ont pu fêter le titre avec leurs supporters, contrairement à 2020, lorsque leur précédent sacre avait été éclipsé par la pandémie de Covid-19. Le joueur de Liverpool Mohamed Salah célèbre son quatrième but avec ses coéquipiers contre Tottenham, le 27 avril 2025, lors du Championnat d'Angleterre.
Liverpool a offert à ses supporters le sacre et la fête dont ils rêvaient, dimanche 27 avril à Anfield, avec une victoire enflammée contre Tottenham (5-1) synonyme de 20e titre en championnat d'Angleterre, le premier depuis 2020. Le Covid avait privé le peuple rouge d'une célébration méritée, il y a cinq ans, et il n'était pas question de gâcher la première "finale" de cette fin de saison, à domicile. Au coup de sifflet, les larmes des supporters se sont mêlés aux fumigènes et les joueurs ont dansé sur l'entêtant "Freed From Desire" de Gala, avant de se tenir, bras dessus bras dessous, devant le mythique Kop pour un très puissant "You'll Never Walk Alone".
"""


Tu es un journaliste. Rédige trois titres convaincants et uniques pour un article en ligne sur le sujet donné dans le contenu : '{contenu}' en '{language}'. Assure-toi d'incorporer les meilleures pratiques SEO en incluant les mots-clés les plus courants et pertinents du contenu dans chaque titre. Pour chaque proposition, affiche uniquement le résultat dans un objet dictionnaire Python avec 'title' comme chaîne de caractères et 'keywords' comme liste. N'affiche rien d'autre. Inclus les trois résultats dans un objet liste Python comme défini ci-dessous. Format de sortie : [{{"title": "La valeur du titre", "keywords": ["mot-clé1", "mot-clé2", "mot-clé3"]}}, {{"title": "La valeur du titre", "keywords": ["mot-clé1", "mot-clé2", "mot-clé3"]}}, {{"title": "La valeur du titre", "keywords": ["mot-clé1", "mot-clé2", "mot-clé3"]}}]
```


**ADVANCED PROMPT**

```python

# résumé
language = "français"
contenu = """
Liverpool sacré champion d'Angleterre après sa victoire contre Tottenham
Sports. Grâce à sa large victoire 5-1 contre Tottenham dimanche, Liverpool a été sacré champion d'Angleterre. Cette fois, ils ont pu fêter le titre avec leurs supporters, contrairement à 2020, lorsque leur précédent sacre avait été éclipsé par la pandémie de Covid-19. Le joueur de Liverpool Mohamed Salah célèbre son quatrième but avec ses coéquipiers contre Tottenham, le 27 avril 2025, lors du Championnat d'Angleterre.
Liverpool a offert à ses supporters le sacre et la fête dont ils rêvaient, dimanche 27 avril à Anfield, avec une victoire enflammée contre Tottenham (5-1) synonyme de 20e titre en championnat d'Angleterre, le premier depuis 2020. Le Covid avait privé le peuple rouge d'une célébration méritée, il y a cinq ans, et il n'était pas question de gâcher la première "finale" de cette fin de saison, à domicile. Au coup de sifflet, les larmes des supporters se sont mêlés aux fumigènes et les joueurs ont dansé sur l'entêtant "Freed From Desire" de Gala, avant de se tenir, bras dessus bras dessous, devant le mythique Kop pour un très puissant "You'll Never Walk Alone".
"""

prompt_example = f"""
Given the input text in '{language}': Input: '{contenu}' Produce a summary of the text in '{language}'.
The summary must be in the same language from the original text in '{language}'.
Captures the main ideas and key points of the text.
Summary Does not include verbatim sentences from the original text. For the proposal,
print only the result in a Python dictionary object with the summary as a string.
Include the all result into a Python list object like define below. Output Format: [ {{"summary": "The summary of the content"}}]
"""
```



**ADVANCED PROMPT**
```python
# PROMPT_3 : Générer le résumé dans une {language} avec une longueur spécifique {summary_length}


# résumé en 5 lignes
language = "français"
contenu = """
Liverpool sacré champion d'Angleterre après sa victoire contre Tottenham
Sports. Grâce à sa large victoire 5-1 contre Tottenham dimanche, Liverpool a été sacré champion d'Angleterre. Cette fois, ils ont pu fêter le titre avec leurs supporters, contrairement à 2020, lorsque leur précédent sacre avait été éclipsé par la pandémie de Covid-19. Le joueur de Liverpool Mohamed Salah célèbre son quatrième but avec ses coéquipiers contre Tottenham, le 27 avril 2025, lors du Championnat d'Angleterre.
Liverpool a offert à ses supporters le sacre et la fête dont ils rêvaient, dimanche 27 avril à Anfield, avec une victoire enflammée contre Tottenham (5-1) synonyme de 20e titre en championnat d'Angleterre, le premier depuis 2020. Le Covid avait privé le peuple rouge d'une célébration méritée, il y a cinq ans, et il n'était pas question de gâcher la première "finale" de cette fin de saison, à domicile. Au coup de sifflet, les larmes des supporters se sont mêlés aux fumigènes et les joueurs ont dansé sur l'entêtant "Freed From Desire" de Gala, avant de se tenir, bras dessus bras dessous, devant le mythique Kop pour un très puissant "You'll Never Walk Alone".
"""

summary_length = 5
prompt_example = f"""
Given the input text in '{language}': Input: '{contenu}' Produce a '{summary_length}' sentences length summary of the text in '{language}'.
The summary must be in the same language from the original text in '{language}'.
Captures the main ideas and key points of the text. Summary Does not include verbatim sentences from the original text.
For the proposal, print only the result in a Python dictionary object with the summary as a string and the summary_length keywords as a integer.
Include the all result into a Python list object like define below.
Output Format: [ {{"summary": "The summary of the content", "summary_length": summary_length_number }}]
"""
```

**ADVANCED PROMPT**


```python
# PROMPT_4 : Depuis un contenu en  {language} , générer 3 tweets de 280 caractéres et 3 hashtags en  {language}

# faire en générer 3 tweets de 280 caractéres et 3 hashtags en  {language}
language = "français"
contenu = """
Liverpool sacré champion d'Angleterre après sa victoire contre Tottenham
Sports. Grâce à sa large victoire 5-1 contre Tottenham dimanche, Liverpool a été sacré champion d'Angleterre. Cette fois, ils ont pu fêter le titre avec leurs supporters, contrairement à 2020, lorsque leur précédent sacre avait été éclipsé par la pandémie de Covid-19. Le joueur de Liverpool Mohamed Salah célèbre son quatrième but avec ses coéquipiers contre Tottenham, le 27 avril 2025, lors du Championnat d'Angleterre.
Liverpool a offert à ses supporters le sacre et la fête dont ils rêvaient, dimanche 27 avril à Anfield, avec une victoire enflammée contre Tottenham (5-1) synonyme de 20e titre en championnat d'Angleterre, le premier depuis 2020. Le Covid avait privé le peuple rouge d'une célébration méritée, il y a cinq ans, et il n'était pas question de gâcher la première "finale" de cette fin de saison, à domicile. Au coup de sifflet, les larmes des supporters se sont mêlés aux fumigènes et les joueurs ont dansé sur l'entêtant "Freed From Desire" de Gala, avant de se tenir, bras dessus bras dessous, devant le mythique Kop pour un très puissant "You'll Never Walk Alone".
"""


prompt_example = f"""
You are a smart and intelligent community manager.
Craft three compelling messages of 280 characters each for an online post in {language} about the topic given in the content in {language}.
Ensure to incorporate Social Media Optimization (SMO) best practices by including the most common keywords from the content.
For each proposal in {language}, print only the result in a Python dictionary object with 'message' as a string and 'hashtags' as a list of hashtags.
In the list of hashtags, for each hashtag, do not forget to add the sign "#" in front of it e.g. "hashtags": ["#hashtag1", "#hashtag2", "#hashtag3"].
Include all results into a Python list object as defined below.
Output Format:[{{"message": "The value of the message", "hashtags": ["#hashtag1", "#hashtag2", "#hashtag3"]}}, {{"message": "The value of the message", "hashtags": ["#hashtag1", "#hashtag2", "#hashtag3"]}}, {{"message": "The value of the message", "hashtags": ["#hashtag1", "#hashtag2", "#hashtag3"]}}] Content: '{contenu}'
"""
```

