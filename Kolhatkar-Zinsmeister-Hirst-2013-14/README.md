### Information on the ASN corpus

Copyright_protected_ASN_corpus.json contains annotated data for anaphoric occurrences of 
shell nouns in the New York Times (NYT) Corpus. The data was annotated using CrowdFlower (now figure eight), 
which internally uses AMT along with other crowdsourcing channels.

Refer the following publications for our annotation methodology. 

- Varada Kolhatkar, Heike Zinsmeister, and Graeme Hirst. 2013. [Annotating anaphoric shell nouns with their antecedents.](http://aclweb.org/anthology/W/W13/W13-2314.pdf) In Proceedings of the 7th Linguistic Annotation Workshop and Interoperability with Discourse, pages 112–121, Sofia, Bulgaria, August. Association for Computational Linguistics.

- Varada Kolhatkar, Heike Zinsmeister, and Graeme Hirst. 2013. [Interpreting anaphoric shell nouns using antecedents of cataphoric shell nouns as training data.](http://www.anthology.aclweb.org/D/D13/D13-1030.pdf) In Proceedings of the 2013 Conference on Empirical Methods in Natural Language Processing, pages 300–310, Seattle, Washington, USA, October. Association for Computational Linguistics.

The annotated file contains annotated data in json format. Each json object has the 
following attributes.
 
1. id: an identifier
2. title: the title of the article in the NYT corpus 
3. sentence: the sentence annotated by the crowd in the first stage of annotation
4. anaphor: the anaphoric shell noun phrase in the given context. (We can't include the 
   text itself because of copyright issues. It should not be too hard to retrieve the text 
   from the NYT corpus. The *title* and *sentence* attributes could be useful in this 
   process.) 
5. antecedent[0-9]: list of antecedents annotated by crowd annotators. Each antecedent 
   follows the format antecedent:confidence, where the antecedent is the textual 
   antecedent selected by the crowd and confidence is the CrowdFlower confidence with 
   which that antecedent was chosen. 

Please do not distribute this data without our permission. Write to us at 
kvarada@cs.ubc.ca, if you have any questions. 
