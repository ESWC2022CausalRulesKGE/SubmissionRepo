# Content

This repository contains, for the submission to ESWC2022 :
- our data (in both rdf and tsv, as we used the tsv file for training our embedding models)
- the mined rules (pdf)

# How to read MinedRules.pdf

This document present a simplified version of the rules representation.

In this table, the resulting effect is that :
X1 wants to reduce its meat consumption more than X2.

Several columns are to be read :
- Path : represents the final property path for the treatment
- ValueX1 and ValueX2 : values for x1 and X2 on the path
- OddsRatio_Lower : lower bound of the confidence interval (build at 80%)

Several rules can be fead :
- if Node == None : then the treatment is to be read X1 has ValueX1 and X2 has ValueX2
- if Node != None : then (i) X1 has the Node and X2 does not or (ii) X1 agrees with the node while X2 do not
