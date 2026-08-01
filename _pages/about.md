---
permalink: /
title: "About"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a Ph.D. student in the Department of Computer & Information Sciences at University of Delaware, where I work with [Prof. Ilya Safro](https://www.eecis.udel.edu/~isafro/index.html) in the [Algorithms, AI & Computational Science Lab](https://safroresearch.blogspot.com/). I am currently a Research Aide at Argonne National Laboratory.

:microscope: My current research involves machine learning for quantum computing, specifically on combinatorial optimization, quantum compilation, with applications in power systems (i.e. unit commitment). Before working on quantum computing, I focused on safety-aware and robust AI modeling. (I made the switch in Jan 2025).

:mortar_board: I obtained my B.S. at Texas Christian University.

News
======
* [Jul 2026] Two papers accepted to QCE'26
* [Apr 2026] Joined Argonne National Lab as Research Aide
* [Mar 2026] Passed Qualifying Exam :tada:
* [Oct 2025] Rejoined Fujitsu Research of America Quantum Lab as Research Intern
* [Jul 2025] Paper accepted to QCE'25
* [Jun 2025] Joined Fujitsu Research of America Quantum Lab as Research Intern
* [Dec 2024] Two papers accepted to AAAI'25
* [Sep 2024] Paper accepted to NeurIPS'24
* [Jul 2024] Participated in UD ATOM Hackathon
* [Jul 2024] Paper accepted to CIKM'24
* [Jul 2023] Participated in UD DS + AI Hackathon
* [Jul 2023] Paper accepted to CVIU'23, Volume 235

What I'm Working On
======
My current research focuses on developing machine learning techniques to improve the quantum computing stack.
- **Cross-Problem Setting for Quantum Approximate Optimization Algorithm (QAOA)**
  ![title image](http://nyquixt.github.io/images/cross-problem.png "Title")
  - *Parameter transferability in QAOA.* A key challenge in scaling QAOA lies in finding good variational parameters, especially for hard instances. The goal is to build machine learning models that can learn transferable patterns from simple problem instances (i.e. from native unconstrained MaxCut) and generalize them to harder ones (i.e. constrained MIS), effectively minimizing expensive optimization.
  - *Problem-aware Graph Representation.* To aid the parameter generation for quantum circuit, a meaningful, problem-aware graph embedding is required to condition the machine learning meta-learner. The generalized Quadratic Programming formulation is used to generate a heterogeneous graph as the input to a HeteroGNN that learns to minimize the QP surrogate loss via unsupervised learning.
  - *Cross-Problem Parameter Generation for QAOA.* A meta-optimizer is trained to predict parameter trajectory for a QAOA circuit, conditioned on the problem-aware graph embedding. It is observed to achieve better performance that unconditioned meta-optimizer that often collapse to near-identical trajectories across instances.
- **Quantum Compilation**
  ![qap router image](http://nyquixt.github.io/images/qap-router.png "QAP-Router")
  - *Qubit Routing on Quantum Device.* The NP-hard problem is viewed as a dynamic quadratic assignment problem. A QAP-solution-aware policy network is trained with a reinforcement learning framework where the QAP objective is integrated into the reward function.
  - *Qubit Assignment & Scheduling on Distributed Quantum Device.* [Work in Progress...]
- **Application in Power Grid Systems.**
  ![uc pce image](http://nyquixt.github.io/images/uc-pce.png "UC-PCE")
  - *Time-dependent Unit Commitment.* To tackle the time-dependent Unit Commitment formulation, Pauli-Correlation Encoding is used for compact qubit representation. The variational quantum circuit is then optimized using a bi-level optimization procedure in a leader-follower structure.

<b>TLDR;</b> I aim to bridge machine learning with quantum algorithm design to make quantum optimization more scalable, robust, and ultimately impactful for real-world applications.

Selected Publications
======
<u><b>Quantum Era</b></u>

* [Graph-Conditioned Meta-Optimizer for QAOA Parameter Generation on Multiple Problem Classes](http://nyquixt.github.io/files/qce26-paper1.pdf). <b>Kien X. Nguyen</b> and Ilya Safro. <i>In Proceedings of the IEEE Quantum Computing and Engineering</i>, 2026.

* [Q3SAT-GPT: A Generative Model for Discovering Quantum Circuits for the 3-SAT Problem](http://nyquixt.github.io/files/qce26-paper2.pdf). Pratim Ugale, Ilya Tyagin, Karunya Shirali, <b>Kien X. Nguyen</b>, and Ilya Safro. <i>arXiv</i>, 2026.

* [Cross-Problem Parameter Transferability in Quantum Approximate Optimization Algorithm: A Machine Learning Approach](http://nyquixt.github.io/files/qce25-paper.pdf). <b>Kien X. Nguyen</b>, Bao Bach, and Ilya Safro. <i>In Proceedings of the IEEE Quantum Computing and Engineering</i>, 2025.

<u><b>Pre-Quantum Era</b></u>

* [Interpretable Failure Detection with Human-Level Concepts](http://nyquixt.github.io/files/aaai25-1-paper.pdf). <b>Kien X. Nguyen</b>, Tang Li, and Xi Peng. <i>In Proceedings of the AAAI Conference on Artificial Intelligence</i>, 2025 (Oral).

* [Adaptive Cascading Network for Continual Test-time Adaptation](http://nyquixt.github.io/files/cikm24-paper.pdf). <b>Kien X. Nguyen</b>, Fengchun Qiao, and Xi Peng. <i>In the 33rd ACM International Conference on Information and Knowledge Management</i>, 2024.
