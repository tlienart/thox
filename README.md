# Thesis

(if you happen to be interested, send me an email at `tlienart £ turing > ac > uk`)

## Structure

* (cover page with compressed abstract)
* Title page with logo and co (no supervisors)
* Acknowledgements (*single space*)
* Abstract (*single space*)
* TOC (*single*)
* (List of Figures)
* Notations (single)
* General Intro (what is it about, bayesian inference, how is the document structured and why (explain software project at ATI))
* **Part I** (sampling methods)
    * Intro
        * Basic MC estimators, importance sampling, validation (ESS, Computational effort)
        * Intro to SMC-sampling and filtering        
        * Intro to PDMP-sampling (global one)
        * Discussion
    * TFS
        * The smoothing problem + litt review
            * FFBS and TFS + difference
        * The Backward Information smoother
            * GTFS and BIS, subsampling
            * (variance, log partition function?)
            * experiments
        * Discussion
    * LBPS and applications
        * The local BPS
            * (comparison with HMC on a chain)
            * (comparison with TFS on HMM?)
        * Application of the local BPS (PMF)
        * Discussion
* **Part II** (message passing algorithms)
    * Intro
        * Belief Propagation / message passing
            * BP, BP on a tree, notion of message, link with Kalman
            * LBP, problems advantages
        * Variational inference
            * VB with mean field style assumption
            * VI in the exponential family (basic form): ADF
            * EP, EP fixed point, EP energy (not in details)
        * Discussion
    * EPBP
        * PBP and the problem
        * EPBP: method and properties
        * Experiments
        * (Generalisation)
        * Discussion
    * SNEP
        * EP mixing with MCMC, SMS
        * Updates in the mean parameter space and SNEP
        * Experiments
        * Discussion
* General Conclusion, perspectives
    * (discuss Bayesian ML in general, bring rant from bayesian comp)
    * sampling vs message passing, pros cons and blah
* Appendices
* Bibliography (*single*)

## Todo

### Research

* investigate use of LBPS

### Writing

* write more about SNEP + your own way
* skip blah from body and shove it in technical intro
* discuss why only consider marginals (see same discussion in W&J08), discuss alternatives (SMC on GM, Naesseth etc)

### Formatting

* pick notation for messages (with/without arrow), use it throughout. Leaning for without. Requires a comma in HMM setting. Arrows are confusing for pre-message.
* itsep should be the same everywhere
* consistency: lower case *expectation propagation* and *belief propagation*
* caption of algorithms: blue/not
* pass @ end to fix image placement ignore until publish time (add fig on individual pages)
* if only very few propositions/theorems, maybe don't use
* hunt for `(??)` in last pass.

## Useful tex resources

* citation with theorem: http://tex.stackexchange.com/questions/36918/how-can-one-cite-theorems-of-references
