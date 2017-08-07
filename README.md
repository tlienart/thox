# Thesis

![stability-wip](https://img.shields.io/badge/stability-work_in_progress-lightgrey.svg)

(if you happen to be interested, send me an email at `tlienart £ turing > ac > uk`)

## Todo

### Research

* comparison HMC, LBPS, BPS, Gibbs for PMF

### Writing

* skip blah from body and shove it in technical intro
* discuss why only consider marginals (see same discussion in W&J08), discuss alternatives (SMC on GM, Naesseth etc)
* **style**: try to remove "we do this" then "we do that" which is a bit too informal. (leave that kind of comments to supervisors as well)

### Conventions

* use `d` for dimension of parameters
* use `n` for ambient dimension
* use `N` for number of points
* use `K` for number of factors
* use `theta` for global approximation
* use `lambda` for cavity parameters
* use `omega` for local parameters
* use `nu` for base measure

### Formatting

* pick notation for messages (with/without arrow), use it throughout. Leaning for without. Requires a comma in HMM setting. Arrows are confusing for pre-message.
* itsep should be the same everywhere (and probably not as huge as Latex wants it to be) use `\itsepa`
* consistency: lower case *expectation propagation* and *belief propagation*
* caption of algorithms: blue/not
* pass @ end to fix image placement ignore until publish time (add fig on individual pages)
* if only very few propositions/theorems, maybe don't use
* hunt for `(??)` in last pass.
* hessian -> Hessian
* check for irregular spaces after `\subsubsections`
* check for huge white spaces after/before algorithms, figures, tables, anything really significantly ugly.
* use we mostly, don't use things like "consider now" but rather "Let us now" blah

## Useful tex resources

* citation with theorem: http://tex.stackexchange.com/questions/36918/how-can-one-cite-theorems-of-references

# STRUCTURE

* () (cover page with compressed abstract)
* (++) Title page with logo and co (no supervisors)
* () Acknowledgements (*single space*)
* () Abstract (*single space*)
* (+) TOC (*single*)
* () (List of Figures)
* (++) Notations (single)
    * (++) Notations / symbols / conventions
    * (+) Abbreviations
* () General Intro (what is it about, bayesian inference, how is the document structured and why (explain software project at ATI))
    * () Objectives, bayesian inf, structure
    * (+) Markov Random Fields
* **Part I** (sampling methods)
    * Background
        * (+) Basic MC estimators, importance sampling, validation (ESS, Computational effort)
        * () Intro to SMC-sampling and filtering
        * () Intro to PDMP-sampling (global one)
        * () Discussion
    * TFS
        * () The smoothing problem + litt review
            * () FFBS and TFS + difference
        * () The Backward Information smoother
            * () GTFS and BIS, subsampling
            * () (variance, log partition function?)
            * () experiments
        * () Discussion
    * LBPS and applications
        * () The local BPS
            * () (comparison with HMC on a chain)
            * () (comparison with TFS on HMM?)
        * () Application of the local BPS (PMF)
        * () Discussion
* **Part II** (message passing algorithms)
    * Background
        * () Variational Inference
            * () General form (discuss alpha div, KL, KStein, Wasserstein)
            * () VB, mean field, ELBO, Guarantees (and lack thereof)
        * (++) Expectation propagation
            * (++) Exponential family and convexity
            * (++) ADF and EP (not in details)
        * () Belief Propagation / message passing
            * () BP, BP on a tree, notion of message, link with Kalman
            * () LBP, problems advantages
        * () Discussion
    * EP for Distributed Bayesian Inference
        * (+) Distributed Bayesian Inference
        * (++) EP variants for distributed inference
            * (++) Damped updates in the natural parameter space
            * (++) Damped updates in the mean parameter space
            * (++) The EP energy perspective
            * (++) Mirror descent for the EP energy
        * () Comparisons
        * () Discussion
    * EPBP
        * () PBP and the problem
        * () EPBP: method and properties
        * () Experiments
        * () (Generalisation)
        * () Discussion
* () General Conclusion, perspectives
    * () (discuss Bayesian ML in general, bring rant from bayesian comp)
    * () sampling vs message passing, pros cons and blah
* () Appendices
* (+) Bibliography (*single*)
