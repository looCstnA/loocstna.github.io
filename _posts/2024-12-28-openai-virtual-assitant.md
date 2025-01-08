---
layout: post
title: Comment Créer un Assisant Personel
subtitle: 
permalink: /assistant-virtuel/
description: >-
  Guide sur la création d'assisant personel avec OpenAI et ChatGPT
author: Gautier
date: 2024-12-21 18:00:00 +0100
categories: [Liste]
tags: [Intelligence Artificielle, Education]
top: 1
excerpt_image: "/assets/images/icons/schoolbus_icon.gif"
---


```text
⚠️ Cette page est encore en construction.
📣 N'hésitez pas à me faire parvenir vos commentaires.

Dernière mise à jour: 07/01/2025

Gautier
```

ChatGPT, l'application qui a pris le monde par surprise.

<img src="/assets/images/application_chatgpt.jpg">

Deux points important à retenir ici: 

- ChatGPT peut "halluciner", c'est-à-dire inventer des choses et ce à chaque instant. 
- ChatGPT comme beaucoup d'application collecte vos données et ce à chaque instant aussi.

N'oubliez jamais qu'il a été entrainer sur les données "publiques" trouvées sur internet et sur internet, depuis son avenement commercial en 1993, [personne ne sait que vous êtes un chien](https://fr.wikipedia.org/wiki/On_the_Internet,_nobody_knows_you%27re_a_dog){:target="_blank"}.

<img src="https://upload.wikimedia.org/wikipedia/en/f/f8/Internet_dog.jpg">

En bref, sur internet, n'importe qui peut poster n'importe quoi. Ceci reste vrai sur votre téléphone. Il existe aujourd'hui de nombreuses applications de Chat ou autres qui se basent sur les modèles GPT d'OpenAI (voir la capture suivante), et celles-ci ont la main mise sur toutes les données qui transitent entre vous et ChatGPT, veillez donc à sélectionner cautioneusement les applications que vous utilisez.

<img src="assets/images/chatgpt_on_play.jpg">

Mais revenons à ChatGPT, celui-ci offre par défault tout une série d'applications, ou d'utilisations pour ne pas confondre avec l'application même, de ses modèle GPTX.

- Création d'image
- Résumer un text ou un document
- Rédaction de contenu
- Recommandations ou avis
- Création de plan
- Echange d'idées


[OpenAI.com](https://openai.com), la société derrière ChatGPT fourni un terrain de jeux pour quiconque (nous verrons que ce n'est pas encore réellement pour n'importe qui) désirant mettre en place diverses fonctions ou applications en lien avec les modèles que OpenAI offre.

Que trouve-t-on dans la platforme mise à disposition par OpenAI?

Nous y trouvons :

- Le **Chat**: L'équivalent technique ou scientifique de ChatGPT 
- **Realtime**: l'équivalent parlé de ChatGPT. 
- **Assistants**: qui permet aujourd'hui trois choses: l'interprétation de code, la recherche de fichier, ou recherche sémantique, et l'appel de fonction.
- **TTS**, l'acronyme de Text-To-Speech en anglais, ou la génération de parole (audio) à partir de texte.
- **Completions**, qui n'est finalement que le chat présenté différement et qui est voué à disparaître du playground, cette partie sera néanmoins toujours disponible via l'API de OpenAI.

<img src="/assets/images/openAI_playground.png">

Nous développerons ici plus bas le Chat, nous développerons les autres fonctionnalités, plus avancées ou plus technique, dans un un article future.

Nous y trouvons aussi l'accès à un forum de practiciens et ingénieurs et des [cookbooks](https://cookbook.openai.com/) ou recettes en français a diverses fins:

- traduction de voix en divers langages
- Narration de vidéo
- Créer un moteur de recherche de type sémantique
- des techniques pour améliorer la fiabilité des résultats
- comment calibrer des modèles de chat
- etc.

Ces recettes sont très fortement orientées d'un point de vue technique et s'adressent encore à un public technique lui aussi.

Prenons par exemple cet article, [Custom LLM as a Judge](https://cookbook.openai.com/examples/custom-llm-as-a-judge) qui décrit comment utiliser un LLM afin de juger (noter) de la qualité de réponse donnée à des questions prédéfinie. Cette recette décrit le code utilisé afin en mettre en palce des technologies qui elles aussi sont principalement des outils d'ingénieurie technique.

- Parlez vous Python, ou n'importe quel langage de programmation?

## Le Chat

Nous allons donc tout d'abord nous intéresser à l'application principale, qui est le point de départ des autres fonctionalités disponibles, le **chat**.

<img src="/assets/images/openAI_playground.png">

Nous y trouvons deux éléments prinicpaux:

- la discussion, au centre de l'écran
- les paramètres, à droite

Nous ne le voyons pas encore sur la capture d'écran ci-dessus, mais la discussion fait intervernir trois éléments du Chat:

- le système
- l'utilisateur (nous ici)
- l'assistant (voir la capture suivante)

<img src="/assets/images/openai_chat_assistant.png">

Avez-vous trouvé la différence avec la capture précédente?

Nous nous mettons ici dans le rôle de l'assistant, c'est-à-dire que nous pouvons nous même définir les réponses de ChatGPT aux questions ou éléments de la discussion.