---
title: "Determining the parent and associated fragment formulae in mass spectrometry via the parent subformula graph"
collection: publications
category: manuscripts
permalink: /publication/2023-11-07-Paper-2
excerpt: 'This paper concerns a novel method of assessing the plausibility of "parent" molecular formulae, by first using it to annotate fragment formulae and then using the annotations to construct what we call a "parent subformula graph" (PSG). Then, the plausibility of the parent molecular formulae is expressible by a simple metric on the PSG.'
date: 2023-11-07
venue: 'Journal of Cheminformatics'
#slidesurl: 'http://academicpages.github.io/files/slides2.pdf'
#paperurl: 'http://academicpages.github.io/files/paper2.pdf'
citation: 'Sean Li, Björn Bohman, Gavin R. Flematti, Dylan Jayatilaka (2023). &quot;Determining the parent and associated fragment formulae in mass spectrometry via the parent subformula graph.&quot; <i>J. Cheminform </i>. 15(104).'
---
# Abstract:

## Background

Identifying the molecular formula and fragmentation reactions of an unknown compound from its mass spectrum is crucial in areas such as natural product chemistry and metabolomics. We propose a method for identifying the correct candidate formula of an unidentified natural product from its mass spectrum. The method involves scoring the plausibility of parent candidate formulae based on a parent subformula graph (PSG), and two possible metrics relating to the number of edges in the PSG. This method is applicable to both electron-impact mass spectrometry (EI-MS) and tandem mass spectrometry (MS/MS) data. Additionally, this work introduces the two-dimensional fragmentation plot (2DFP) for visualizing PSGs.

## Results

Our results suggest that incorporating information regarding the edges of the PSG results in enhanced performance in correctly identifying parent formulae, in comparison to the more well-accepted “MS/MS score”, on the 2016 Computational Assessment of Small Molecule Identification (CASMI 2016) data set (76.3 vs 58.9% correct formula identification) and the Research Centre for Toxic Compounds in the Environment (RECETOX) data set (66.2% vs 59.4% correct formula identification). In the extension of our method to identify the correct candidate formula from complex EI-MS data of semiochemicals, our method again performed better (correct formula appearing in the top 4 candidates in 20/23 vs 7/23 cases) than the MS/MS score, and enables the rapid identification of both the correct parent ion mass and the correct parent formula with minimal expert intervention.

## Conclusion

Our method reliably identifies the correct parent formula even when the mass information is ambiguous. Furthermore, should parent formula identification be successful, the majority of associated fragment formulae can also be correctly identified. Our method can also identify the parent ion and its associated fragments in EI-MS spectra where the identity of the parent ion is unclear due to low quantities and overlapping compounds. Finally, our method does not inherently require empirical fitting of parameters or statistical learning, meaning it is easy to implement and extend upon.