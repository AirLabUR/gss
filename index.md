# <center>Music Source Separation with Generative Flow</center>

<center>Ge Zhu<sup>1</sup>, Jordan Darefsky<sup>1</sup>, Fei Jiang<sup>2</sup>, Anton Selitskiy<sup>1</sup>, and Zhiyao Duan<sup>1</sup></center>
<center><sup>1</sup>AIRLab (University of Rochester), <sup>2</sup>XX</center>


## Abstract

<div style="text-align: justify"> Music source separation under full supervision,
where paired mixed signals and source signals are both available,
has obtained substantial progress over the years. However, this
setting highly relies on large amounts of paired data. Source-only
supervision, on the other hand, decouples the process of learning
a mapping from a mixture to particular sources into a two
stage paradigm: source modeling and separation. Recent systems
under source-only supervision either achieve good performance
in synthetic toy experiments or limited performance in music
separation task. In this paper, we leverage flow based generators
to train music source priors and likelihood based objective to
separate music mixtures. Experiments show that in both singing
voice and music separation tasks in MUSDB18 dataset, our
proposed systems achieve competitive results to one of the full
supervision systems. We also demonstrate one variant of our
proposed systems is capable of separating new source tracks
effortlessly.</div> 

<br>

![arch](images/diagramv3.png)

<br>
