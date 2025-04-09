---
permalink: /
title: "About"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Since January 2025, I am a postdoctoral researcher at CISPA Helmholtz Center for Information Security, working with [Julian Loss](https://www.julianloss.com/).

Previously, I was a PhD student at the Institut de Recherche en Informatique Fondementale [IRIF](https://www.irif.fr/), Université Paris Cité, under the supervision of [Geoffroy Couteau](https://geoffroycouteau.github.io/) and [Alain Couvreur](http://www.lix.polytechnique.fr/Labo/Alain.Couvreur/).
My subject was "Multiparty Computation from the Hardness of Coding Theory", and you can find my thesis [here](https://theses.hal.science/tel-04889558/)

 More generally, my research interests lie in Secure Multiparty Computation, and Pseudorandomness Generation, Coding Theory, and general foundation of cryptography. You can find my CV [here](/CV_Clement_Ducros.pdf).

Publication
======

- FOLEAGE: F4OLE-Based Multi-Party Computation for Boolean Circuits, *Dung Bui, Maxime Bombar, Geoffroy Couteau, Clément Ducros and Sacha Servan-Schreiber*, ASIACRYPT 2024 ([ePrint](https://eprint.iacr.org/2024/429.pdf),[Springer](https://link.springer.com/chapter/10.1007/978-981-96-0938-3_3)).
<details>
  <summary><em style="margin-left: 10px;">Abstract</em></summary>
  <p  style="margin-left: 20px;"><em> ecure Multi-party Computation (MPC) allows two or more parties to compute
any public function over their privately-held inputs, without revealing any information be-
yond the result of the computation. Modern protocols for MPC generate a large amount of
input-independent preprocessing material called multiplication triples, in an offline phase. This
preprocessing can later be used by the parties to efficiently instantiate an input-dependent
online phase computing the function.
To date, the state-of-the-art secure multi-party computation protocols in the preprocessing
model are tailored to secure computation of arithmetic circuits over large fields and require
little communication in the preprocessing phase, typically O(N ·m) to generate m triples among
N parties. In contrast, when it comes to computing preprocessing for computations that are
naturally represented as Boolean circuits, the state-of-the-art techniques have not evolved since
the 1980s, and in particular, require every pair of parties to execute a large number of oblivious
transfers before interacting to convert them to N -party triples, which induces an Ω(N 2 · m)
communication overhead.
In this paper, we introduce F4OLEAGE, which addresses this gap by introducing an efficient
preprocessing protocol tailored to Boolean circuits, with semi-honest security and tolerating
N − 1 corruptions. F4OLEAGE has excellent concrete performance: It generates m multiplication
triples over F2 using only N · m + O(N 2 · log m) bits of communication for N -parties, and can
concretely produce over 12 million triples per second in the 2-party setting on one core of a
commodity machine. Our result builds upon an efficient Pseudorandom Correlation Generator
(PCG) for multiplication triples over the field F4. Roughly speaking, a PCG enables parties to
stretch a short seed into a large number of pseudorandom correlations non-interactively, which
greatly improves the efficiency of the offline phase in MPC protocols. This is achieved by intro-
ducing a number of protocol-level, algorithmic-level, and implementation-level optimizations on
the recent PCG construction of Bombar et al. (Crypto 2023) from the Quasi-Abelian Syndrome
Decoding assumption.</em></p>
</details>


-  Correlated Pseudorandomness from the Hardness of Quasi-Abelian Decoding, *Maxime Bombar, Geoffroy Couteau, Alain Couvreur, and Clément Ducros* in CRYPTO 2023 ([ePrint](https://eprint.iacr.org/2023/845.pdf),[Springer](https://link.springer.com/chapter/10.1007/978-3-031-38551-3_18))

- Pseudorandom Correlation Functions from Variable-Density LPN, Revisited, *Geoffroy Couteau and Clément Ducros*, in PKC 2023 ([ePrint](https://eprint.iacr.org/2023/650.pdf),[Springer](https://link.springer.com/chapter/10.1007/978-3-031-31371-4_8))


We may have met - Events and Talks
======

I have participated in the following events, in the antichronological order:
- [Journée C2 2025](https://barracuda.inria.fr/fr/),  Pornichet, March 30th to April 4th, 2025
- [CWI Seminar](https://projects.cwi.nl/crypto/),  CWI - Amsterdam , September 9th to September 13th, , 2024
- [EUROCRYPT 2024](https://eurocrypt.iacr.org/2024/), Zurich , May 26th to May 30th, 2024
- [PEPR-SecureCompute](https://www.pepr-cybersecurite.fr/projet/securecompute/), ENS ULM - Paris, January 24th, 2024
- [Rennes Crypto Seminar](https://www.creachlabs.fr/en/seminars-keeping-date-latest-research/cryptography-seminar),  IRMAR - Université de Rennes, January 19th, 2024
- [Journées C2 2023](https://indico.math.cnrs.fr/event/9364/), Najac, October 15th to October 20th, 2023.
- [CRYPTO 2023](https://crypto.iacr.org/2023/), Santa Barbara, August 19th to August 24th, 2023.
- [EPIT 2022](https://epit2023.sciencesconf.org/), June 12th to June 16th, 2023.  
- [PKC 2023](https://pkc.iacr.org/2023/), Atlanta, May 7th to May 10th, 2023.
- [EUROCRYPT 2023](https://eurocrypt.iacr.org/2023/), Lyon, April 23th to April 27th, 2023.
- [Retraite ANR Barracuda 2023](https://barracuda.inria.fr/fr/), Mortagne-sur-Gironde, January 8th to January 13th, 2023.
- [ICALP 2022](https://icalp2022.irif.fr/), Paris, July 4th to July 8th, 2022.
- [Retraite ANR Barracuda 2022](https://barracuda.inria.fr/fr/), Metabief, June 27th to July 1st, 2022.
- [TPMPC 2022](https://www.multipartycomputation.com/tpmpc-2022), Aarhus, June 7th to June 10th, 2022.
- [EUROCRYPT 2022](https://eurocrypt.iacr.org/2022/), Trondheim, May 30th to June 3rd, 2022.
- [Journées C2 2022](http://jc2-2022.inria.fr/fr/), French Workshop for PhD students, Hendaye, April 10th to April 15, 2022.




