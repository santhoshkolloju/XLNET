# XLNET 
<h3>Generalized Auto Regressive Pre Training For Language Modelling </h3>

BERT (Bi-directional encoder representation from Transformer) has stayed on the State Of 
Art(SOA) for a really long time.This was the real image net moment in the area of Natural 
language processing. But one of the major drawbacks of BERT was the fixed context(it can 
only allow a sentence up to a length of 512) though they have the potential to learn long
term dependency. Transformer-Xl was proposed to learn the dependency beyond the fixed length
context. It consists of a segment level recurrence mechanism and a novel positional encoding 
scheme. Incorporating the pro's of both  the models a new novel architecture is propose called
XL-NET which outperforms BERT on 20 tasks  by large margin.


Langauge Modelling On a high level can be divivded into two types:
<ul>
<li>Auto Regression Based Approach</li>
<li>Density Based Approach</li>
</ul>

<b>Auto-Regressive language modeling (ARM)</b> tends to estimate the probability distribution of a text corpus with an
autoregressive model. Specifically, give a set of tokens ARM tends to find the probability P(Wi|Wi-1,Wi-2....W1) 
or the other way around (backward modeling) and then minimizes the cross-entropy loss. But ARM is not effective in deep bidirectional context's which are required for many downstream tasks. This is the reason ARM is not effective in pre training for transfer learning.
