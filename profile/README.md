# Aurora

**Virtual spatial transcriptomics from H&E images.**

Spatial transcriptomics is costly and low-throughput, so it reaches only a small
fraction of routine histology and the molecular state of disease goes unmeasured
in most patients.

Aurora predicts it instead. DeepSpot-M reads an H&E slide and returns
transcriptome-wide expression on that slide's own coordinates. No assay is run,
and no tissue is consumed.

Most programmes hold H&E for every case and spatial data for almost none. Start
from the slides you already hold. Screen them, then spend the next assay where
the question is sharpest.

Aurora is a research platform built on research from ETH Zurich, the University
of Zurich and the University of Basel.

A prediction is a hypothesis about what an assay would have measured. It is not
a measurement, it is not evidence about a patient, and it has no clinical use.

## Start here

Two repositories take a slide to a result. Each one is a worked example you can
run and then lift into your own code.

| Repository | What it covers |
| --- | --- |
| [deepspot-h-quickstart](https://github.com/auroraomics/deepspot-h-quickstart) | A slide, its tiles, and the embeddings, computed on your own machine. |
| [deepspot-m-quickstart](https://github.com/auroraomics/deepspot-m-quickstart) | Embeddings or a slide to virtual spatial transcriptomics, then spatial expression, UMAP and clustering. |

New to the platform? [Install and prepare a slide](https://docs.auroraomics.org/quickstart/)
is the first page of the documentation, and
[Send a slide, get a result](https://docs.auroraomics.org/first-prediction/)
is the path end to end.

## The two models

**DeepSpot-H** is the foundation model for H&E images. It turns each tile of
your slide into one embedding.
[What DeepSpot-H reads and returns](https://docs.auroraomics.org/models/deepspot-h/).

**DeepSpot-M** is the model that predicts spatial gene expression. It turns
those embeddings into spatial gene expression.
[What DeepSpot-M reads and returns](https://docs.auroraomics.org/models/deepspot-m/).

## Choose how your data reaches us

DeepSpot-H can run on your machine or on ours. DeepSpot-M only ever runs on
ours. That choice is what the two routes are.

**Your slides stay with you.** Run DeepSpot-H on your own machine and send the
numbers it produces. Every image stays local.

What leaves is a few hundred numbers per tile, the tile's position and the
quality measurements that kept it.
[Run DeepSpot-H locally](https://docs.auroraomics.org/guides/embeddings/).

**Send your slides.** Send image tiles when images may leave your machine.
Aurora handles the model-side processing when the catalogue lists a compatible
model. [Check whether your slide fits](https://docs.auroraomics.org/use-cases/is-this-for-my-slide/).

## Access

Analysis is for academic and non-profit research. Commercial evaluation and use
run under a separate written agreement, which starts at
[auroraomics.org/contact](https://auroraomics.org/contact).

The hosted API takes a key. A key is minted for an account granted programmatic
access that has accepted the current Terms.

A request is reviewed by a person, and preparing a sample needs no account. The
two run side by side.

[Get access](https://docs.auroraomics.org/get-access/) is the whole procedure.
[Limits](https://docs.auroraomics.org/limits/) states every quota counter and
size cap a key is held to.

## Where to go

| | |
| --- | --- |
| Website | <https://auroraomics.org> |
| Documentation | <https://docs.auroraomics.org> |
| API | <https://api.auroraomics.org/v1/> |
| Platform status | <https://auroraomics.org/api/health> |
| Try it on a prepared sample | <https://auroraomics.org/demo> |
| Whole documentation site in one fetch | <https://docs.auroraomics.org/llms.txt> |

## Papers and data

- [DeepSpot-M: a multimodal foundation model for transcriptome-wide virtual
  spatial transcriptomics from histology](https://www.medrxiv.org/content/10.64898/2026.06.19.26356060v1).
  The model behind Aurora. medRxiv, 2026.
- [DeepSpot: Leveraging Spatial Context for Enhanced Spatial Transcriptomics
  Prediction from H&E Images](https://www.medrxiv.org/content/10.1101/2025.02.09.25321567).
  The predecessor method. medRxiv, 2025.
- [TCGA Virtual Spatial Transcriptomics Atlas](https://huggingface.co/datasets/ratschlab/TCGA_virtual_spatial_transcriptomics_atlas).
  12TB and 295M+ spots, predicted from H&E with DeepSpot-M.

## Licensing

Example code in the quickstart repositories above is MIT, so you can lift a cell
into your own analysis.

The `auroraomics` package is published under a non-commercial licence, which the
[documentation names and links](https://docs.auroraomics.org/quickstart/). Model
weights carry their own separate terms, which the model's card names.

## Responsible use

[Responsible use](https://docs.auroraomics.org/responsible-use/) states the
conditions the Terms attach to every result.

[Privacy and retention](https://docs.auroraomics.org/privacy/) states what is
stored, for how long, and what deleting a job removes.
