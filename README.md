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

## Repository contents

This repository contains the organized scripts, modules, and analytical pipelines used in our study. The codebase is structured to cover the entire computational workflow, from initial data processing to complex network analysis and model implementation:

| Module / Directory | Description |
|---|---|
| **Single-cell RNA sequencing data preprocessing** | Foundational pipelines for QC, filtering, and initial processing of raw single-cell sequencing data. |
| **Dimensionality reduction clustering and dataset integration** | Scripts for UMAP/t-SNE embedding, graph-based clustering, and batch-effect correction across multiple datasets. |
| **scRNA-seq-analysis-of-the-reprogramming-screening-Experiment** | Dedicated analysis workflow specific to the combinatorial reprogramming screening experiments. |
| **Gene expression analysis and visualization** | Tools for differential gene expression evaluation, marker identification, and generation of manuscript-quality figures. |
| **Principal Component and Correlation Analysis** | Statistical modules for evaluating global transcriptional shifts and feature-level correlations. |
| **Pseudotime Analysis and Differentiation Potential Estimation** | Advanced trajectory inference tools to map developmental progression and cell fate potential. |
| **Regulatory network analysis with SCENIC** | Inference and analysis of transcription factor regulons and gene regulatory networks. |
| **model** | Relevant information regarding the ReproPerturb approach. |

## Intended use

ReproPerturb is designed for research use in computational biology, stem cell engineering and perturbation-response modelling. The materials in this repository are provided to help readers understand the analytical framework, evaluate the data processing workflows, and explore the biological applications described in our study.

## Availability

This repository provides the computational pipelines and scripts corresponding to the findings presented in our study. For specific questions regarding the analytical workflows, codebase components, collaboration inquiries, or access to associated materials, please contact the corresponding authors listed in the manuscript.

## Citation

If you refer to ReproPerturb before formal publication, please cite the associated manuscript as:

> A context-dependent virtual cell framework maps reprogramming plasticity and captures a self-renewing OCT4+ human hypoblast stem cell state. Manuscript submitted.

A complete citation, DOI and publication link will be added when available.

