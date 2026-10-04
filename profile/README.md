# Aurora

**Building the virtual molecular layer for tissue biology.**

Aurora predicts spatial gene expression from routine H&E images, helping
researchers explore molecular patterns across samples, cohorts and disease.

## What you can do

- [Explore the whole archive on the same predicted genes](https://auroraomics.org/use-cases/annotate-an-archive),
  and keep measured follow-up for the hypotheses that survive.
- [Rank the candidate samples on predicted expression](https://auroraomics.org/use-cases/choose-what-to-sequence),
  and choose where each capture area goes.
- [Add the sample's bulk RNA profile to the prediction for its slide](https://auroraomics.org/use-cases/add-a-bulk-profile),
  and keep the same genes and file format.
- [Predict the genes your panel left out](https://auroraomics.org/use-cases/extend-a-panel),
  on the spots it measured, then choose which leads to validate.
- [Adapt the model to your protocol from a few measured slides](https://auroraomics.org/use-cases/adapt-to-your-cohort),
  or restore genes that failed quality control as labelled predictions.

[Explore research applications](https://auroraomics.org/use-cases) on the website.

## Where to start

- **Upload a slide on the website.** Aurora Direct takes an H&E image and an
  email address, with no code and no account.
  [Submit images for analysis](https://auroraomics.org/upload), or
  [explore the example slide](https://auroraomics.org/demo).
- **Work from code** with [Aurora Docs](https://docs.auroraomics.org). The API
  and the Python package let you submit samples and read predictions without
  the browser.
- **[deepspot-h-quickstart](https://github.com/auroraomics/deepspot-h-quickstart)**
  runs DeepSpot-H on one H&E slide, on your own machine.
- **[deepspot-m-quickstart](https://github.com/auroraomics/deepspot-m-quickstart)**
  follows one H&E slide to its predicted spatial gene expression, and explores
  the result.

## The models behind a prediction

**DeepSpot-H** is the foundation model for H&E images.
[Learn about DeepSpot-H](https://docs.auroraomics.org/models/deepspot-h/).

**DeepSpot-M** is the model that predicts spatial gene expression.
[Learn about DeepSpot-M](https://docs.auroraomics.org/models/deepspot-m/), or
[read the paper](https://www.medrxiv.org/content/10.64898/2026.06.19.26356060v1).

## Choose the workflow that fits your research

- **[Send your slides](https://docs.auroraomics.org/quickstart/).** Prepare
  your H&E slide on your own machine and send its tiles.
- **[Your slides stay with you](https://docs.auroraomics.org/guides/embeddings/).**
  Run DeepSpot-H on your own machine and send the numbers it produces.

[From slide to result](https://docs.auroraomics.org/first-prediction/) follows
one H&E slide to its spatial gene expression result.

---

For research use only. Aurora is not a medical device.
[Terms apply](https://auroraomics.org/terms).
