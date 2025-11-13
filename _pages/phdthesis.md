---
layout: archive
title: "Phd Thesis"
permalink: /phdthesis/
author_profile: true
---


From October 2021 to November 2024, I was a PhD student in University Paris-Cité (IRIF lab, Algocomp team), under the supervision of Alain Couvreur and Geoffroy Couteau. I defended the thesis on November 12 2024.

The jury included:

- Nico Döttling (President of the jury, Professor, Helmholtz Center for Information Security (CISPA)).
- Nicolas Sendrier (Reviewer, \\ Research Director, INRIA Paris).
- Emmanuela Orsini (Reviewer, Tenure-Track Assistant Professor, \\ Bocconi University).
- Yixin Shen (Examiner, Research Scientist, INRIA \\ Rennes).
- Philippe Gaborit (Examiner, Professor, CNRS, University of Limoges).
- Lisa Kohl (Examiner, Researcher, CWI, Amsterdam, The Netherlands).
- Sophie Laplante (PhD director, Professor, Université Paris-Cité, IRIF, Paris)
- Alain Couvreur (PhD co-director, Research Director, INRIA Saclay, Paris)
- Geoffroy Couteau (PhD co-director, Researcher, CNRS, IRIF, Paris)

The thesis can be found [here](/thesisDucros.pdf). 




## Thesis summary


My thesis tackles a sub-area of the great art that is cryptography: it focuses on the question of secure multiparty computation. The question raised by this field is straightforward: can different parties, each holding private data, compute functions over these hidden inputs without leaking any private information during the process? The question itself is appealing, but what is even better is that it can be done.

For several years, however, this positive result was somewhat overshadowed by the impossibility of obtaining practical MPC. By this, I mean MPC that could be developed and deployed widely, something we could imagine using in everyday life. MPC applications are numerous and have, in my opinion, been insufficiently considered in public debates about privacy protection, even though they provide remarkably strong security guarantees. The high costs—especially in communication, but also computation—were a major obstacle, preventing even basic awareness that MPC could become a practical tool.

With this in mind, research advanced quickly, and my PhD was motivated by important discoveries: the invention of two related primitives, Pseudorandom Correlation Generators (PCGs) and Pseudorandom Correlation Functions (PCFs). Since the very beginning of MPC (which roughly coincides with the early days of modern cryptography), it has been known that if parties receive in advance certain well-chosen random correlations—that is, random values related in specific ways across the parties—then these additional correlations significantly enhance MPC protocols, making them efficient in practice. But one problem remained: how can parties obtain all the random correlations they need without relying on a trusted dealer? Protocols that allowed the parties themselves to generate these correlations did exist, but they suffered from two major issues: (1) the non-negligible cost of generating even a single correlation, which caused scalability problems, and (2) the huge number of correlations typically required for standard MPC applications.

PCGs and PCFs answer this problem: they allow parties to obtain a large number of correlations with low computational cost and, more importantly, with communication that grows only logarithmically in the number of correlations produced.

In the thesis, we present several PCG constructions whose security relies on variants of the Syndrome Decoding (SD) assumption, a classical assumption in coding theory. The intuition behind these constructions is to merge the SD assumption with MPC techniques that enable additively sharing sparse vectors. The thesis demonstrates constructions that were state-of-the-art at the time, for secure multiparty computation protocols involving more than two players when the computation is over a finite field of size greater than 2. We also show how to remove this constraint at the cost of a small communication overhead.

We also study a construction of PCFs. The main conceptual difference compared to PCGs is that, in a PCF, the parties can obtain their correlations “on the fly”: they hold correlated functions whose outputs, when evaluated on the same input, are themselves correlated. These objects offer more flexibility than PCGs but are also more difficult to construct. Again, we rely on variants of the SD assumption. We build on a previous PCF construction, show that the associated security proof was incorrect, and propose a corrected proof. Additionally, we present optimizations based on a better analysis and precise parameter tuning through simulations. We achieve parameters that are usable in practice.

Finally, this thesis revolves around the use of certain codes, particularly those underlying the SD assumption. The search for good complexity requires finding the most efficient codes while ensuring that security is not compromised. We consider a framework tailored to the study of promising attacks on SD and its variants. For each construction mentioned above, we conduct a thorough security analysis of the associated SD variant and carry out cryptanalysis efforts to compute concrete parameters.
