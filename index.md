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

<table align="center">
  <thead>
    <tr>
      <th> </th>
      <th>Reference Voice</th>
      <th>LUT Sample</th>
      <th>D-vector Sample</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Female Singer1</th>
      <td><audio controls="" preload="auto">
            <source src="demo/GT/vocals.wav"></audio></td>
      <td><audio controls="" preload="auto">
            <source src="demo/GT/bass.wav"></audio></td>
      <td><audio controls="" preload="auto">
            <source src="demo/GT/drums.wav"></audio></td>
    </tr>
    <tr>
      <th>Female Singer2</th>
      <td><audio controls="" preload="auto">
            <source src="wavs/inset_ref/238.wav"></audio></td>
      <td><audio controls="" preload="auto">
            <source src="wavs/inset_emb/lut_238.wav"></audio></td>
      <td><audio controls="" preload="auto">
            <source src="wavs/inset_dvec/dvec_238.wav"></audio></td>
    </tr>
    <tr>
      <th>Female Singer3</th>
      <td><audio controls="" preload="auto">
            <source src="wavs/inset_ref/1161.wav"></audio></td>
      <td><audio controls="" preload="auto">
            <source src="wavs/inset_emb/lut_1161.wav"></audio></td>
      <td><audio controls="" preload="auto">
            <source src="wavs/inset_dvec/dvec_1161.wav"></audio></td>
    </tr>
    <tr>
      <th>Male Singer1</th>
      <td><audio controls="" preload="auto">
            <source src="wavs/inset_ref/658.wav"></audio></td>
      <td><audio controls="" preload="auto">
            <source src="wavs/inset_emb/lut_658.wav"></audio></td>
      <td><audio controls="" preload="auto">
            <source src="wavs/inset_dvec/dvec_658.wav"></audio></td>
    </tr>
    <tr>
      <th>Male Singer2</th>
      <td><audio controls="" preload="auto">
            <source src="wavs/inset_ref/1189.wav"></audio></td>
      <td><audio controls="" preload="auto">
            <source src="wavs/inset_emb/lut_1189.wav"></audio></td>
      <td><audio controls="" preload="auto">
            <source src="wavs/inset_dvec/dvec_1189.wav"></audio></td>
    </tr>
    <tr>
      <th>Male Singer3</th>
      <td><audio controls="" preload="auto">
            <source src="wavs/inset_ref/1512.wav"></audio></td>
      <td><audio controls="" preload="auto">
            <source src="wavs/inset_emb/lut_1512.wav"></audio></td>
      <td><audio controls="" preload="auto">
            <source src="wavs/inset_dvec/dvec_1512.wav"></audio></td>
    </tr>
  </tbody>
</table>
