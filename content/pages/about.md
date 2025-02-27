Title: About the Journal
Slug: about
              
<div id="scope"/>
About the Journal
----------------------
**ISSN:** 2744-6204
<!-- ### Directory-->
1. [Scope](#scope)
2. [Philosophy](#philosophy)
3. [Definitions](#definitions)
***       
<h3>Scope</h3>
*Physiome* publishes articles describing physiological models which demonstrate that the mathematical model, model implementation, and simulation results are consistent and reproducible. *Physiome* articles must be linked to primary papers published in or accepted to a peer-reviewed physiology, bioengineering or biophysics journal.

Submissions must include sufficient information that independent *Physiome* curators are able to evaluate the consistency and reproducibility of the model, its implementation, and the simulations that are performed in producing the simulation results.
***
<h3 id="philosophy"><i>Physiome</i> Philosophy</h3>
Scientific research pushes the boundaries of human knowledge, but for knowledge to be useful, reproducibility and reuse must be core values. Reproducibility as confirmation of results should be one of the supporting pillars of good research. Yet, the demonstration and publication of reproducibility is rarely incentivised, and is often treated as a secondary result at best, which undermines the quality of our collective work. With the strict formulation of equations and easily shareable code, one would think that mathematical models should be reproducible by default. However, when tested by the <a href="http://reproduciblebiomodels.org"  target="_blank" rel="noopener noreferrer">Center for Reproducible Biomedical Modeling</a>, less than 5<span>&hairsp;</span></td></tr>% of the models published in scientific journals could be implemented by another group. *Physiome* is a journal committed to reproducibility and reusability of mathematical models of physiological processes. A *Physiome* publication is a complement to your primary article that ensures reproducibility, reusability and discoverability of your model.

*Physiome* articles describe the details of mathematical models and computational simulations associated with a ‘primary’ experimental/modelling paper that has been published (or accepted for publication) in a peer-reviewed physiology, bioengineering or biophysics journal. Submissions to *Physiome* are evaluated to determine their reproducibility, reusability, and discoverability. At a minimum, accepted submissions are guaranteed to be in an executable state that reproduces the modelling predictions in the primary paper, and are archived for permanent open access by the community. *Physiome* articles are published on <a href="http://physiome.figshare.com/"  target="_blank" rel="noopener noreferrer">figshare</a> as a PDF manuscript containing all the information needed to run the implementation of the model, and an <a href="http://co.mbine.org/standards/omex"  target="_blank" rel="noopener noreferrer">OMEX archive</a> containing the model implementation (which can be opened by any type of zip reader). 

Physiological modelling typically evolves with a workflow similar to the following:

<ol>
<li> carry out experiments
<li> formulate a model based on anatomy, physiology, & physics
<li> translate the physiology/physics into mathematical equations
<li> implement these equations in computational code
<li> run the code to produce simulation results and predictions
<li> compare predictions with experiments and iterate steps 2-6 until the model matches the experiments (i.e. validate the model)
<li> publish the experimental data, the equations, and the predictions, sometimes with the code provided as supplemental information
</ol>

Traditionally, scientific journals in this domain will publish the experimental data (1) and predictions (5) without strictly checking that the code (4) really does match the published model (2) or the simulation results (5) (although reviewers may check this if sufficient information is provided). Their focus is typically on the validation and verification (6) of the model.

We are now seeing various efforts aiming to address model and simulation reproducibility, see for example the <a href="http://reproduciblebiomodels.org"  target="_blank" rel="noopener noreferrer">Center for Reproducible Biomedical Modeling</a>. Such efforts focus on ensuring that model implementation (4) and simulation results (5) are consistent and reproducible.

The goal of *Physiome* is to encourage model authors to make their models available in a manner that is reusable. To achieve this, the *Physiome* curation process aims to verify that the model (3), model implementation (4) and simulation results (5) are all consistent and reproducible.

The purpose of *Physiome* is to encourage the reproducibility and reuse of models by providing citation credit for papers that document and make available curated and annotated models - thus making the models truly <a href="https://www.go-fair.org/fair-principles/"  target="_blank" rel="noopener noreferrer">FAIR</a>. As such, the journal encourages the use of appropriate standard formats for encoding models and simulations. The journal will assist authors in making suitable submissions available in the *Physiome* encoding standards (<a href="https://www.cellml.org/"  target="_blank" rel="noopener noreferrer">CellML</a>, <a href="http://www.fieldml.org/"  target="_blank" rel="noopener noreferrer">FieldML</a>, <a href="http://sbml.org/"  target="_blank" rel="noopener noreferrer">SBML</a>, <a href="https://www.neuroml.org/"  target="_blank" rel="noopener noreferrer">NeuroML</a> for encoding the model; <a href="http://sed-ml.org/"  target="_blank" rel="noopener noreferrer">SED-ML</a> for encoding the simulation protocols, parameters and outputs). Where no suitable standards exist for a given model and/or simulation experiment, the implementation of the model needs to be provided in such a way that the *Physiome* curators are able to evaluate the reproducibility of the submission.

To encourage best practice we propose to assign one of four levels to a *Physiome* paper, as follows: 
<ol>
<li>The model is reproducible and implemented in the way described in the primary paper. This is the minimum requirement for a <i>Physiome</i> paper</li>
<li>The model is coded in one of the <a href="http://co.mbine.org/"  target="_blank" rel="noopener noreferrer">COMBINE standards</a> such as <a href="https://www.cellml.org/"  target="_blank" rel="noopener noreferrer">CellML</a>, <a href="http://sbml.org/"  target="_blank" rel="noopener noreferrer">SBML</a> or <a href="https://www.neuroml.org/"  target="_blank" rel="noopener noreferrer">NeuroML</a>. For models encoded in CellML, this allows the model to be checked automatically for consistency of units, and allows for the automatic generation of the mathematical equations behind the model and their translation to multiple languages (Python, Matlab, C, C++, Fortran, etc.)</li> 
<li>The model code is consistent with the mathematical description of the model</li>
<li>The model obeys physical laws such as conservation of energy and conservation of mass or charge. For a lumped parameter model, this generally means that it has been implemented in bond graph form. For a partial differential equation continuum model, it means that the model has been formulated as a port-Hamiltonian system and implemented numerically in a mass and energy conserving form.</li>     
</ol>
Ideally, all models would reach level 4; we realise that this is unrealistic, at least in the short term. We hope that over time the *Physiome* community will increasingly come to expect models to adopt these high standards and that software will be developed to make it easier for authors to achieve that goal. 
<div align="right"><h4><a href="#about"><i class="fa fa-angle-double-up"></i></a></h4></div>
***
<h3 id="definitions">Definitions</h3>


A model simulation is **repeatable** when re-running it produces a consistent result. 

A model is **reproducible** when its outputs can be reproduced by a machine from an unambiguous statement of the model equations, together with specified values of the model parameters, initial conditions and boundary conditions. Markup languages such as <a href="https://www.cellml.org/"  target="_blank" rel="noopener noreferrer">CellML</a>, <a href="http://sbml.org/"  target="_blank" rel="noopener noreferrer">SBML</a>, <a href="https://www.neuroml.org/"  target="_blank" rel="noopener noreferrer">NeuroML</a> and <a href="http://www.fieldml.org/"  target="_blank" rel="noopener noreferrer">FieldML</a> are designed to encode a model in unambiguous form. The markup language <a href="http://sed-ml.org/"  target="_blank" rel="noopener noreferrer">SED-ML</a> is designed to specify the simulation protocol for running the model with specified inputs and outputs.

A model is **reusable** when it can be used as an independent model or as a module within another model. This requires that the appropriate use of the model is well documented and that its limitations are clear, and that the model is semantically annotated to provide the biological and biophysical meaning of all of its variables and components. One of the goals of the *Physiome* Project is to encourage modular approaches to modeling to facilitate the reuse of well documented and validated modules.

A model is **discoverable** when it has been annotated with metadata that describe the purpose and use of the model sufficiently to allow the model to be retrieved via a webservice.

A model is **validated** when its predictions under specified conditions match experimental observations.

<div align="right"><h4><a href="#about"><i class="fa fa-angle-double-up"></i></a></h4></div>









