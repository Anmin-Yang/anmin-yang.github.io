---
layout: page
title: Natural language processing of narrative writing for depression screening in adolescents
description: a machine-learning approach to predict mental status from single piece of composition 	
img: assets/img/projects/nlp/paradigm.png
importance: 6
category: past
---

Psychology has a longstanding belief that the words and content one chooses to express are not random but rather a reflection of the hidden state of one's mental world. The famous **Freudian Slip** suggests that a verbal or memory mistake is believed to reveal an unconscious belief, thought, or motive. The **Thematic Apperception Test (TAT)** follows a similar assumption by analyzing one's thought to an ambiguous or open-end stimuli. 

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/projects/nlp/fig1_freudian.png" title="freudian slip" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/projects/nlp/fig2_TAT.png" title="TAT" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left, Freudian Slip. Right, Thematic Apperception Test.
</div>

While those methods have deep roots in psychology, they are often accused of **bad inter-rater reliability** and **doubtful validity**. On the other hand, although questionaires are considered the standard of clinical diagnosis, for particular cohorts, in our case, adolescents, the self-report measure may be potentially biased due to factors such as limited language skills, life experiences, cognitive impairments, and the social expectancy bias. This study aims to find more **ecological**, age-appropriate and psychologically appropriate depression detection methods for adolescents.

We used students’ compositions written in the classroom to detect depression among adolescents.

For **feature extraction**, we employed both theory-based and data-driven approach:

- LIWC (Linguistic Inquiry and Word Count)
- Word2Vec

For **classifiers**, we used:

- classic machine learning approach
  - Logistic Regression
  - SVM
- deep neural networks
  - TextCNN
  - TextRNN

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="../assets/img/projects/nlp/paradigm.png" title="scheme" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Schematic illustration of the computational models.
</div>

The textRNN model achieved the best performance with F-measure at 0.74.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="../assets/img/projects/nlp/fig3_rnn.png" title="rnn" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Performance of TextCNN and TextRNN
</div>

Our research highlights the potential of natural language processing techniques in detecting depressive tendencies in young populations at school.

**See our work** at [PsyArXiv](https://psyarxiv.com/5f9nb/)