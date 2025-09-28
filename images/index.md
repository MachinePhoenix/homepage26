---
title: "D2-RST: Dual-Dimensional Residual Side Tuning for Mitigating Feature Forgetting in Parameter-Efficient Transfer Learning"
authors:
- admin
- Yaoming Wang
- Wenrui Dai
- Jiarui Zhang
- Ziyang Zheng
- Chenglin Li
- Junni Zou
- Hongkai Xiong

author_notes:

date: "2025-02-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: ""

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["preprint"]

# Publication name and optional abbreviated publication name.
publication: "WACV 2026"
publication_short: ""

abstract: "Existing fine-tuning methods for pre-trained models, including parameter-efficient transfer learning (PETL) approaches, suffer from severe feature forgetting in deep layers due to progressive spectral decay. To address this issue, we present \textbf{Dual-Dimensional Residual Side Tuning (D2-RST)}, a novel PETL framework designed to mitigate feature forgetting by jointly optimizing aggregated features, i.e., residuals, across both embedding and spatial dimensions. Specifically, D2-RST employs a dual-block side tuning structure: Collect Blocks extract inter-layer information into residuals while Feed Blocks strategically reintegrate them back into the backbone. This parallel processing framework with low-rank linear mappings applied to residuals effectively stabilizes low-frequency components while reducing memory cost. Additionally, D2-RST introduces a spatial-dimension pathway in parallel with the conventional feature-dimension pathway, followed by cross-dimensional fusion via learnable scalars at each Feed Block, thereby effectively suppressing low-frequency attenuation in deeper layers. To further reduce redundancy, we propose a parameter-sharing strategy for LoRA matrices within Collect Blocks, where low-rank projections are shared across multiple layers. Extensive experiments on several benchmarks demonstrate that D2-RST not only outperforms existing PETL methods in accuracy but also significantly reduces parameter overhead by explicitly suppressing deep-layer feature forgetting."

# Summary. An optional shortened abstract.
summary: PETL, Side-tuning, ViT.

# tags:
# - Source Themes
featured: false

links:
# - name: Custom Link
#   url: http://example.org
url_pdf: D2-RST.pdf
# url_code: ''
# url_dataset: ''
# url_poster: ''
# url_project: ''
# url_slides: ''
# url_source: ''
# url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: ''
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
# projects:
# - internal-project

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example
---

<!-- {{% callout note %}}
Create your slides in Markdown - click the *Slides* button to check out the example.
{{% /callout %}}

Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://wowchemy.com/docs/content/writing-markdown-latex/). -->
