# LLM-Scored-23

This repository contains the additional data for the paper titled "An Empirical Study on Using Large Language Models to Analyze Software Supply Chain Security Failures". 

There are 5 files in this repository. 

1. articles.py:
Contains all the articles in the catalogue used as the dataset for the study.\
For example, 'article1' contains the content of the first article in the catalogue (sorted by the most recent article).\
The catalogue being referred to here is a collection of articles on software supply chain failures collected by CNCF.\
The link to this catalogue: https://github.com/cncf/tag-security/tree/main/supply-chain-security/compromises

3. GptPrompts.py:                                                                       
This file contains the code for prompting GPT 3.5's response to the various prompts used in the paper.\
There are functions for each dimension:\
type()- runs the prompt for all articles for the dimension 'type of compromise'. \
impacts()- is for the dimension 'impacts'\
nature()- is for the dimension 'nature'\
solution()- is for the dimension 'Solutions/learnings'\
intent()- is for the dimension 'intent'\

4. BardPrompts.py:
This file contains the code for prompting GPT 3.5's response to the various prompts used in the paper.\
The function 'classification()' contains all the prompts for Bard. Various variables contain the different prompts.\
For example, 'intent_prompt' contains the prompt for the intent dimension and so on. 
   
5. Classifying articles-analysis.xlsx
This Excel file contains the manual labelling by the raters for each article.\
It also contains the calculation for both the accuracy of GPT (GPT analysis) and Bard (Bard analysis).\

6. Appendix.pdf: 
This pdf contains the appendix for the paper with the relevant tables and figures.\
