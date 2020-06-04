# tribAIn

<img src="https://github.com/snow0815/tribAIn/blob/master/documentation/tribAIn.png" height="200.5" width="575">

## About

The tribAIn<a href="#footnote1" id="footnote1ref"><sup>1</sup></a> ontology aims to formalize knowledge gained from tribological experiments for reuse, comparison and documentation. Therefore, the tribAin ontology provides concepts for the specification of methodological background knowledge of experimental design, the documentation of the experimental setup and the representation of different kinds of results (e.g. measurements series, analysis, interpretation in natural-language). Using the EXPO<a href="#footnote2" id="footnote2ref"><sup>2</sup></a> (ontology of scientific experiments) as basis, gives tribAIn a generic background about scientific experimental design, methodology and results representation.

<a id="footnote1" href="#footnote1ref"><sup>1</sup><a> *Derived from the ancient Greek word “tribein” (= rubbing) and the acronym “AI” (= Artificial Intelligence)*  
  <a id="footnote2" href="#footnote2ref"><sup>2</sup><a> *Soldatova, L. N.; King, R. D. An ontology of scientific experiments. Journal of the Royal Society, 631 Interface, 2006, 11, pp. 795–803. 10.1098/rsif.2006.0134*
    
## Background

Carrying out experiments in the domain of tribology usually involves the three steps experimental design, experimental procedure and experimental results and is highly-based on background knowledge from domain experts. Reuse and comparison of results and knowledge gained from scientific experiments  requires a common basis in all three steps, which is provided by methodology, standardized procedures and routines.

<img src="https://github.com/snow0815/tribAIn/blob/master/documentation/ProcessExperiments.png" height="345.5" width="771.5">

First, the domain expert has to choose a suited experimental design including the fabrication of test samples suited to the assessed experimental model (system structure), the definition of a target variable, their influence on friction and wear beahvior is studied, and the kinematical and operational parameters.
Second, the experimental proedure is frequently carried out by standardized testing devices, producing comparable measurement series as output files (e.g. in csv format). Since conclusions about friction and wear behavior are based on the comparison of experimental results with those of a reference system, the experimental procedure involves different measurement series with a variation of the value of the target variable.

Finally, experimental results are gained by (statistical) analyses of the measurement series, an interpretation of the results and the documentation. Knowledge gained from conducted experiments is further used as input for a new experimental design.
Reuse and comparison of existing knowledge gained from conducted tribolgical experiments therefore requires a suited representation for methodological background, experimental results and interpretation, which relates the output of the three steps.

## Core Concepts of tribAIn

<img src="https://github.com/snow0815/tribAIn/blob/master/documentation/CoreConcepts.png" height="456" width="743">

The core concepts of tribAIn are modeled according to the background of tribological experiments relating the three areas experimental design, experimental procedure and experimental results. A *Sample* is the center of an investigation, as it represents the real-world entity, which is investigated in an experiment. Experimental design in the domain of tribology results in the definition of a *Tribological Reference Method*, containing information about the system structure and the *Stress Collective*. A Sample is further assessedBy a *Scientific Experiment* using a suited *Device*, which results in output variables in form of *Measurement Series* by a given *Input* set. For a statistical analysis more than one sample is tested under the same conditions, thus these are grouped in *Sample Groups*, for comparing the results with respective those of a *Reference Group*. The interpretation of the analyses and the comparison resultsIn an assertion on *Frictional* and *Wear Behavior* of the investigated tribosystem. The mainly used relation in the tribAIn ontology is the transitive part-of-relationship to sign the membership of an object to an aggregated object.

## Used Material

The ontology-editor Protégé (Version 5.5.0) was used for building the owl representation of tribAin and further test inferencing using the Pellet reasoner. Concepts from the EXPO were used forming the basis for tribAIn.

* [Protégé](https://protege.stanford.edu/) - Musen, M.A. [The Protégé project: A look back and a look forward.](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4883684/) AI Matters. Association of Computing Machinery Specific Interest Group in Artificial Intelligence, 1(4), June 2015. DOI: 10.1145/2757001.2757003.
* [EXPO](https://sourceforge.net/projects/expo/) ontology

## Usage and License

The tribAIn ontology is made available as owl-file and ttl-file for general use and download from this repository.  
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.
