# ReproPerturb

**ReproPerturb** is a context-dependent virtual cell framework for exploring how combinatorial signalling perturbations shape cell fate outcomes during somatic cell reprogramming. The framework integrates baseline cellular states with large-molecule perturbation inputs, including small molecules, growth factors and cytokines, to predict downstream transcriptional responses and cell-type composition in silico.

This repository provides the public-facing project page for ReproPerturb. It is intended to describe the conceptual framework, biological use cases and release status associated with the manuscript currently under consideration. Detailed implementation files, model checkpoints and internal screening scripts are not included in this public landing repository at this stage.

## Overview

ReproPerturb was developed to support systematic interrogation of lineage specification landscapes under high-dimensional combinations of signalling inputs. In the accompanying study, the model was applied to transcription factor-mediated somatic cell reprogramming and used to prioritize perturbation conditions associated with early human lineage outcomes, including hypoblast-like states.

At a high level, ReproPerturb represents cell states and perturbation inputs in a unified latent space and predicts two complementary readouts: **cell-type-specific gene expression profiles** and **cell-type proportions** after perturbation. This design enables large perturbation spaces to be explored computationally before focused experimental validation.

## Key features

| Feature | Description |
|---|---|
| Multimodal perturbation representation | Encodes small molecules and protein factors within a shared representation suitable for combinatorial perturbation modelling. |
| Context-aware virtual cell modelling | Uses baseline cellular states to predict context-dependent transcriptional and compositional responses. |
| Cell-type-resolved prediction | Outputs both lineage-specific gene expression profiles and predicted cell-type abundance shifts. |
| Interpretable latent programs | Links perturbation-associated signalling patterns to latent functional programs and downstream gene-level responses. |
| Large-scale in silico screening | Enables prioritization of candidate perturbation combinations from millions of possible signalling conditions. |

## Biological application

ReproPerturb was used to map perturbation-responsive reprogramming trajectories across multiple early lineage attractors. In the study, this framework helped identify signalling conditions associated with the capture and stabilization of expandable OCT4-positive induced hypoblast stem cells with features of human pre-implantation hypoblast.

The model was also evaluated using independent lineage-directed perturbation conditions and benchmarked against alternative computational perturbation modelling approaches. These analyses support ReproPerturb as a practical framework for hypothesis generation in stem cell engineering and early developmental biology.

## Repository status

This repository is currently maintained as a **project information and release-tracking page**. It contains a concise description of the ReproPerturb framework and will be updated as manuscript, data and software release decisions are finalized.

| Component | Current status |
|---|---|
| Project overview | Available in this README. |
| Manuscript link | To be added upon publication or public preprint release. |
| Processed metadata | Planned for release where compatible with manuscript and data-use policies. |
| Example outputs | Planned for staged release. |
| Source code | Not publicly released in this repository at the present stage. |
| Model checkpoints | Not publicly released in this repository at the present stage. |

## Intended use

ReproPerturb is designed for research use in computational biology, stem cell engineering and perturbation-response modelling. The public materials in this repository are intended to help readers understand the framework and follow future releases. They are not intended to provide a deployable software package or a complete reproduction workflow at this stage.

## Availability

The ReproPerturb implementation and associated model assets are under active organization for controlled and staged dissemination. Additional documentation, release notes and data-access information will be provided following manuscript publication or other public disclosure of the study.

For questions about collaboration or access, please contact the corresponding authors listed in the manuscript.

## Citation

If you refer to ReproPerturb before formal publication, please cite the associated manuscript as:

> A context-dependent virtual cell framework maps reprogramming plasticity and captures a self-renewing OCT4+ human hypoblast stem cell state. Manuscript submitted.

A complete citation, DOI and publication link will be added when available.

