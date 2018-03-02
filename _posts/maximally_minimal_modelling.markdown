---
layout: post
title:  "Maximally minimal modeling"
date:   2018-02-06 20:44:20 -0500
categories: ???
---




*Truth is ever to be found in the simplicity, and not in the multiplicity and confusion of things*

 Isaac Newton

In my first year of grad school, Prof Chris Henley told me Ising was an average student. I was shocked -- the Ising model is famous in physics, one of the cornerstones of statistical mechanics. It was originally introduced as a toy model of ferromagnetic materials, where the magnetic spin of the constituent particles was idealized to be either 'up' or 'down' (in reality the spin can point in any direction). But its full importance came later, when it was used to understand general critical phenomena, universality, and ultimately the renormalization group; well known triumphs of modern physics. Since then, it has found application in fields ranging from social dynamics to neurobiology.

I was curious how such a successful model could have such a humble origin. I found out that the supposedly modest ability of its progenitor was just one of the quirks of its curious history \cite{brush1967history}. For instance, it was Ising's advisor, Lenz, who conceived the model, whereas Ising just carried out the calculations (to his credit, Ising tried to re-christen it the "Lenz-Ising" model, but it didn't stick \cite{niss2005history}). Furthermore, Ising's original paper had a mistake! He correctly showed that in one dimension there was no ferromagnetic transition, but wrongly concluded that this result would hold in three dimensions. 

But perhaps the most significant quirk is that the model wasn't taken seriously. The physicist Stephen Brush writes "it was scorned or ignored by most scientists" for being "greatly over simplified" \cite{brush1967history}. They believed that idealizing the spin vector to a binary value, which made the model solvable, was too unrealistic. The Nobel prize winner Chen Yang said it was "considered an arcane exercise[s], narrowly interesting, mathematically seducing, but of little consequence" \cite{niss2009history}.  Amusingly, this view was shared by Ising, who was said to have been so disenchanted with the model's relevance that he gave up research \cite{brush1967history}! Yet over time this view changed, as the broad utility of the model, stemming from its simplicity, was gradually realized.

I was fascinated that something as important as the Ising model had been so misjudged, and wondered if other scientific work had been too. In my third year, when I became interested in synchronization, I found out it had.

Collective synchronization occurs when a large population of oscillators spontaneously lock their cycles, in spite of dissimilarities in their natural frequencies. This can be thought of as a temporal analogue of the ferromagnetic phase transition in the Ising model. This effect spans many disciplines. In biology, it is seen in discharging pacemaker cells, in chemistry in metabolic cycles of yeast cell suspensions, and in physics in arrays of superconducting Josephson junctions. There are many other examples, too numerous to list here.

Art Winfree first discovered this sync phenomenon when studying biological rhythms \cite{winfree}. In a seminal, eloquent, and inspiring paper he posited that various physiological rhythms are the product of 'the mutual synchronization of myriads of individual oscillatory processes'. However, the individual oscillators he was imagining weren't of the usual, linear variety. Instead they were nonlinear, which made them oscillate with a preferred amplitude and waveform called a limit cycle. How a population of nonlinear oscillators behaved was unknown. Mathematically, this group behavior would be determined by a large system of nonlinear differential equations -- a formidable challenge immune to the usual tools.

But Winfree wasn't deterred. Like Ising -- or rather Lenz -- his approach was to write down an extremely idealized model in the hope of capturing the essential features of the sync phenomenon. It worked. Simulations showed a transition to "striking community synchronization", which due to the simplicity of the model he was able to partially analyze. Kuramoto later made Winfree's model even simpler, resulting in his famous, eponymous model. In a beautiful analysis he solved the model exactly, ultimately leading to the plenitude of attention the model enjoys today. However, similar to the Ising story, both Kuramoto and the rest of the community were initially rather under-enthused with his results.

In my fourth year, I attended a conference organized in Kuramoto's honor. He was unable to travel in person, so instead recounted his model's tale via video \cite{kuramoto_video}. He told us that when he developed the model he was new to nonlinear science, and so was unsure of its worth. He thus sought expert opinion before publishing his results. With endearing honesty and trademark understatement, he said the feedback was "not so encouraging". The experts "showed little interest in his [my] work, and were even critical". They said his results "didn't seem new at all" and that "there were many similar works in mechanical and electrical engineering". 

Dispirited by this negativity, Kuramoto didn't work on the model for five years. He didn't even publish the work beyond a two page article in a conference proceedings. Serendipitously however, this article was seen by Winfree who recognized its importance and described it in his famous book on biological rhythms \cite{winfree}. This gave the Kuramoto model much exposure, ultimately leading to the wide popularity it enjoys today.

I love both this story and the Ising story. I like that Ising blundered when analyzing his model in three dimensions -- it's encouraging that famous scientists make mistakes too -- and I'm amused that Lenz didn't get titular credit. I also like that the experts' disdain made Kuramoto so reluctant to publish; it humanizes him, while also showing that importance can be gravely mismeasured. But what I love most is that the stories illustrate the power of minimal models. Stripping a model down to its barest features really can work. Simplicity makes things tractable, and tractability makes things understandable. Then, like an inverse series of Russian dolls, greater realism can be added to make things quantitative.

This thesis is an homage to this style of work. It explores minimal models of coupled oscillators. It consists of three projects, each of which is an autonomous publication with its own introduction and conclusion. The first two are about the transient behavior of pulse-coupled oscillators. These are idealizations of relaxation oscillators, which communicate with each other by firing sudden pulses. They are often collectively referred to as the Peskin model, since Charlie Peskin first introduced them when studying cardiac pacemaker cells. Since then however they have found application in low-powered radios, sensor networks, and earthquakes dynamics.

As is typical is nonlinear dynamics, traditional research on the Peskin model focuses on the steady state -- usually some form of synchrony. But the approach to the steady state is less studied. Our work focuses on this part of the dynamics: the prelude to synchrony. We show that this looks like an aggregation process, a link which gives us access to new mathematical tools. In spite of this, the nonlinearities in the system make progress difficult. In a barefaced attempt to mimic the minimalism credo, we eliminate these difficulties by making two idealizations. This makes the model exactly solvable, and its analysis constitutes Chapter one.

In the second Chapter, we show that our idealized model captures the essence of the original problem. This insight, along with the exact analysis of our idealized model, lets us derive good approximations to the transient behavior of the Peskin model, our original goal.


%Chapter three is more ambitious. It seeks to wed two similar, but largely separate, fields: swarming and synchronization. In synchronization, oscillators are characterized by their phases, whose influence on each other promotes temporal order. In swarming systems, the degrees of freedom are the individuals' positions, whose interactions trigger spatial assembly. But what happens if these two effects interact? What does spatiotemporal collective behavior look like?




Chapter three is more ambitious. It seeks to wed two similar, but largely separate, fields: swarming and synchronization. In synchronization, the units are characterized by their phases, whose influence on each other promotes temporal order. In swarming systems, the degrees of freedom are the units' positions, whose influence on each other triggers spatial order. But what happens if these two effects interact? In what ways can units with both temporal and spatial degrees of freedom organize themselves?


To answer this question, we study a generalized Kuramoto model where now the elements are free to move around in space as well as in phase. Further, there is a bidirection coupling between their spatial and phase dynamics. We call these entities 'swarmalators' since they swarm and oscillate.

The original motivation for this work was Janus particles \cite{yan2012linking}. These are micrometer sized particles which can be induced to oscillate about their centers of mass using magnetic fields. When in suspension, they are also free to move around in space. The dynamics of the phase (of oscillation about the center of mass) and position of each particle are coupled to each other, and so Janus particles satisfy our proposed definition of swarmalators. 


As detailed in \cite{yan2012linking}, populations of Janus particles display novel collective behavior.  We first considered trying to model Janus particles directly. The equations of motions were however complicated, making analysis seem unlikely. Numerically solving them was an obvious alternative. But as pointed our by my committee member Chris Myers, the complexity of the governing equations would likely obscure the core phenomenology that we wanted to study, namely the interaction between synchronization and swarming. He made the key suggestion that we instead follow the minimalism principle. Thus we developed a minimal model, whose simplicity, as we show, lets us study some of the states of our system analytically. 

\begin{center}
  * * *
  \end{center}

  A final word on minimal modeling. This approach to science, of course, is far from perfect. Not all phenomena are simple, or expressible with elementary mathematics, and so it will often fail. Of course another danger is that the modeler, in his zealotry for simplicity, will over do it. No one would remember even \textit{seeing} a baby, it having been discharged so feverishly with the dishwater. Yet as as evidenced by my heroes Ising, Winfree, and Kuramoto, it pays to be daring. The skillful modeler therefore strikes a balance between intrepitude and overconfidence. As Emanuel Derman puts it,  "A little north of common sense, but south of idolatry, lies the wise use of models".

