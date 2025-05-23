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

The analysis of this study resulted in a finding that the components which are most aligned with specific brain regions are: embeddings from the final layer of SBERT (with right-hemisphere supramarginal gyrus), embeddings from the 2nd layer (with the triangularis in the right-hemisphere inferior frontal gyrus) and embeddings from the 5th layer (with the orbitalis in the right-hemisphere inferior frontal gyrus). The weakest alignment is observed for the attention heads from the first layer and for the triangularis in right-hemisphere inferior frontal gyrus. The overarching conclusion is that the alignment analysis unveils that SBERT is less sensitive to discourse-level structures than to syntactic structures, while the reverse is true for the brain.

The GithHub repository for the project is available click <a href="https://github.com/przemekkubiak/brain-llm-convergence">here</a>. 

References:
<ul>
  <li>Dou, Y., Shu, K., Xia, C., Yu, P. S., & Sun, L. 2021. User Preference-aware Fake News Detection. arXiv [Cs.SI]. Retrieved from http://arxiv.org/abs/2104.12259</li>
  <li>S. Mo Jang, Joon K. Kim. 2018. Third person effects of fake news: Fake news regulation and media literacy interventions. Computers in Human Behavior. Volume 80. Pages 295-302. ISSN 0747-5632. https://doi.org/10.1016/j.chb.2017.11.034.</li>
  <li>Ngai CSB, Singh RG, Yao L. 2022. Impact of COVID-19 Vaccine Misinformation on Social Media Virality: Content Analysis of Message Themes and Writing Strategies. J Med Internet Res. Volume 24(7):e37806. doi: 10.2196/37806. PMID: 35731969; PMCID: PMC9301555. </li>
  <li>Nguyen, V.-H., Sugiyama, K., Nakov, P., & Kan, M.-Y. 2020. FANG: Leveraging Social Context for Fake News Detection Using Graph Representation. Proceedings of the 29th ACM International Conference on Information & Knowledge Management. doi:10.1145/3340531.3412046</li>
</ul>
