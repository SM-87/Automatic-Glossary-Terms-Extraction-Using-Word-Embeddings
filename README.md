# Automatic-Glossary-Terms-Extraction-Using-Word-Embeddings

This repository contains the automatically extracted glossary terms considering only the feature and benefit attributes of the original CrowdRE requirement specifications dataset. The dataset used in our experiments can be viewed in "CrowdRE Requirements Dataset.csv". However, the original CrowdRE dataset is devloped by P. K. Murukannaiah et al. and can be accessed from "The smarthome crowd requirements dataset", https://crowdre.github.io/murukannaiah-smarthome-requirements-dataset/, April, 2017. 

Along with the glossary set, we have also computed and reported the ground truth set for first 100 requirement specifications of the used CrowdRE dataset. In total, we have extracted 304 glossary terms and 95 ground truth terms. The ground truth terms have been computed from our intuition in an unbiased manner as there exists no benchmark standard ground truth, whereas the glossary terms are extracted and included in the final set based on the similarity scores computed from the word embedding based word2vec model. The file "Glossary and Ground Truth Set.csv" highlights the extracted glossary terms and ground truth terms.   

For finding a similar noun phrase and computing the similarity scores, we have used a similar topic related dataset, i.e. Wikipedia Home Automation Category Dataset, "https://en.wikipedia.org/wiki/Category:Home_automation" and extracted the web pages for a depth of two considering the tree structure wikipedia category.  

The file "Similarity Scores.pdf" reports the calculated cosine similarity scores in alphabetical order for the extracted glossary terms (noun phrases) that are included in the final glossary set using our approach. In the final glossary set, we have included those noun phrases which are having a semantic similarity (cosine similarity) score greater than or equal to 0.5. The range of similarity score is between 0 to 1. The scores closer to 1 means that the words are semantically more similar. On the other hand, scores closer to 0 means that the words are less related to each other. On these basis, we have selected and included the noun phrases in the final set considering the similarity score values greater than or equal to 0.5.
