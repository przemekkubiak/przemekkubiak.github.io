---
title: "Graph Neural Networks for Fake News Detection"
excerpt: "Using GNNs to automatically flag fake news by incorporating social network information."
link: http://url-you-want-linked

---

The Internet provides an unprecedented level of connectivity and ease of communication. However, such communication can be characterised by dissemination of fake news, i.e. incorrect, faked, or misleading statements made to be presented as news. The detrimental impacts of fake news are difficult to underestimate: they can be used to undermine informed citizenry, sabotage democratic processes, and promote pseudoscienes (Jang & Kim 2018; Ngai et al. 2022). 

Social media serves as one of the main sources of information for people using the Internet: <a href="[url](https://www.pewresearch.org/journalism/2016/05/26/news-use-across-social-media-platforms-2016/)">Pew Research Center reported in 2016 that up 62% of US citizens get their news from social media</a> . Given the immense complexity and scale of online communication, flagging and removal of fake news on social media can only be done through large-scale computational and statistical models. 

Recent research has investigated fake news detection models incorporating social network information, which have been reported to achieve higher accuracy rate than models focusing only on textual data involving fake news (Dou et al. 2021; Nguyen et al. 2020). Geometric deep learning provides the possibility of efficiently leveraging social context, giving the model ccess to information about how pieces of data like Tweets are propagated in a network of users.

In this example, I am replicating the experimental setup of Dou et al. (2021) to demonstrate the effectiveness of Graph Neural Networks on fake news detections tasks. Dou et al. (2021) model the social network information by encoding past posts of users with text representation techniques and integrating them with news propagation graphs representing engagement on social media. 


{% include figure image_path="assets/images/propagation-graph.png" alt="placeholder image 1" caption="Sample propagation graph. The root node is the news post, and other nodes represent the users who shared the news. Dotted lines represent user engagement embeddings utilised in the model." %}

