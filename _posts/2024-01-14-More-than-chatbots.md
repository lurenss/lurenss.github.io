---
layout: post
title:  Beyond chatbots
date: 2024-01-14 21:01:00
description: Transformers the AI breakthrough
tags: transformers AI breakthrough chatbots
categories: post
---

Even the least tech-savvy person can see that something significant has occurred in the last year, 
the release of ChatGPT on 30-12-2022  to the public and the consequent mass usage is likely to pass from a small fraction of people that play a video game like tetris to the millions of people that play a more advanced videgame like GTA 6 (hopefully in 2025 if Rockstar doesn't make treats :) )
The only difference is the gaming field this took more than 30 years, in the AI field was a lightning strike.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/tris.jpeg" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gta6.gif" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Tris on the left, GTA 6 on the right, the gap is huge
</div>
As a consequence of this,the AI field boiled up once again, and a new gold rush started.
It's important to mention that not only big corporations are involved in this, but also small startups and even single developers of the open source community, fortunatly i say, It's important to avoid the monopoly of big corporations in this field, but this will be maybe topic for another post.

## How this stuff works on high level
The underlying technology that powers up LLMs is called Transformers, it was invented by Google in 2017 (here the [link]([https://arxiv.org/abs/1706.03762]) for the paper) <br>
In order to understand let's assume that our training set is only a single phrase with the following words "I like eat pizza with Marco" and not the entire wikipedia, reddit as did OpenAI.
So basically what does a transformer is given a sequence of word guess the next one, that's it. <br>
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/transformer1.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
At the beginning the transformer it doesn't know anything so it decide to put a random word.
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/transformer2.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
At this point the learning algorithm say to the transformer, Hey jackass you don't have to insert toilet after I like eat but  pizza. So the next time when I ask what is the word that comes after I like eat it will answer with pizza.
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/transformer3.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
So now this new sequence becomes the input of the transformer and it has to guess the next word, so the previous process is iterated and so on.
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/transformer4.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
This is just what does the transform predict the next word, or in Natural Language Processing terms predict the next token, just it.
More text see the transformer and more will be able to produce sophisticated text given a certain sequence.

## Beyond the text
Until now we have seen how the transformer can be used to generate text, but what if we want to use it for something else? <br>
Well It's simple instead of using  word as tokens we can use different things like GPS coordinates, DNA sequences and so on.
Let's take Transportation field where the ability to forecast people trajectories can greatly improve the efficiency and effectiveness of transportation systems. With the availability of a vast dataset of GPS coordinates, the transformer model can be utilized to predict the next GPS coordinate of an individual or group of people based on a sequence of previous coordinates. This advanced predictive capability has the potential to optimize transportation routes, reduce travel time, and enhance overall user experience.
Alternatively, this technique can also be used to produce synthetic data in instances where it is necessary to achieve a specific population size and analyze its characteristics, based on a representative dataset.
Creating another parallelism between videogames and real life, with a transformer based model trained on user GPS coordinates, is tool that is mimicking the actions and behaviors of individuals based on their history, similar to how city builders or management games function, when the player is aware of traffic congestion, He can take the necessary steps to avoid it, like insert a new road or a new bus line.
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/citiesskylin.jpeg" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
<div class="caption">
    A screenshot from Cities Skylines, a city builder game
</div>
What I'm saying is not just something I dreamed up - there are people who are working on it and have shown preliminary results, like in this papers [Generation of individual daily trajectories by GPT-2]([(https://www.frontiersin.org/articles/10.3389/fphy.2022.1021176/full)]) and [Generating Individual Trajectories Using GPT-2 Trained from Scratch on Encoded Spatiotemporal Data]([(https://arxiv.org/pdf/2308.07940.pdf)]).
Instead for DNA sequences there are a lot of applications, for example, we can use it to predict the next nucleotide in a sequence, or to predict the next amino acid in a protein sequence, or to predict the next codon in a DNA sequence. So it is useful for task like sequence analysis, gene expression, here a paper that cover how transformers can be used in this field [Transformer-based models for gene expression prediction]([(https://academic.oup.com/bioinformaticsadvances/article/3/1/vbad001/6984737)]).

In conclusion, the transformer architecture has revolutionized the field of NLP, allowing for the creation of LLMs with the ability to simulate human-like conversation. Through the use of transformers, language models can be trained on vast datasets, allowing for the prediction of the next word or token based on a sequence of previous words. However, the applications of transformers extend beyond chatbots and language generation. Its ability to process and predict various forms of data, such as GPS coordinates and DNA sequences, opens up a world of possibilities in different fields. While there is still much to explore and develop in this area, the potential for transformers is evident and one technology has a great impact in various and different fields it's for sure a sign of that is and it will be more and more important in the future.




