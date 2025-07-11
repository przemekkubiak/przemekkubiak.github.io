---
title: "Language Models and the Brain: Convergence"
excerpt: "Analysing the architectural and functional similarity between the brain and a langauge model."

---

This project attempts to shed light on the differences and similarities between the brain and language models by identifying which components of a language model appear aligned with various regions in the language network. Specifically, this is analysed by comparing the sensitivity of components of a language model and brain regions to specific linguistic features. The research direction is guided by the hypothesis that if a component of a language model and a brain region are more aligned, they exhibit similarities in the kind of linguistic features they attune to. By analysing data from a neuroimaging study of Wehbe et al.(2014) and the representations of the SentenceTransformers (SBERT) language model (Reimersand Gurevych, 2019), I attempt to answer the following research questions:
<ul>
  <li>RQ1. What components of the language modelare most aligned with brain regions?</li>
  <li>RQ2. What components of the language modelare least aligned with brain regions?</li>
  <li>RQ3. What does the alignment between the language model and the brain tell us about howthey process language?</li>
</ul>

{% include figure image_path="assets/images/brains_pipeline.jpg" alt="placeholder image 1" caption="The model structure outlining the analysis process of this project. The left-hand-side corresponds to loading the text data from Wehbe et al. (2014). The bottom tiles represent the fMRI scanning performed by Wehbe et al. (2014), resulting in brain activity data. The top tiles depict the process of converting strings of text into SBERT embeddings. Both brain activity data and SBERT embeddings are then used to predict linguistic features, indicated by the right-hand-side tile.." %}

The analysis of this study resulted in a finding that the components which are most aligned with specific brain regions are: embeddings from the final layer of SBERT (with right-hemisphere supramarginal gyrus), embeddings from the 2nd layer (with the triangularis in the right-hemisphere inferior frontal gyrus) and embeddings from the 5th layer (with the orbitalis in the right-hemisphere inferior frontal gyrus). The weakest alignment is observed for the attention heads from the first layer and for the triangularis in right-hemisphere inferior frontal gyrus. The overarching conclusion is that the alignment analysis unveils that SBERT is less sensitive to discourse-level structures than to syntactic structures, while the reverse is true for the brain.

The GithHub repository for the project is available click <a href="https://github.com/przemekkubiak/brain-llm-convergence">here</a>. 

References:
<ul>
  <li>Nils Reimers and Iryna Gurevych. Sentence-bert: Sentence embeddings using siamese bert-networks. In Proceedings of the 2019 Conference on Empirical Methods in Natural Lan- guage Processing. Association for Computational Linguistics, 11 2019. URL https://arxiv.org/abs/1908.10084.</li>
  <li>Wehbe L, Murphy B, Talukdar P, Fyshe A, Ramdas A, et al. (2014) Simultaneously Uncovering the Patterns of Brain Regions Involved in Different Story Reading Subprocesses. PLoS ONE 9(11): e112575. doi:10.1371/journal.pone. 0112575.</li>
</ul>
