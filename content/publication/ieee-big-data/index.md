---
title: "Research in IEEE Big Data Conference 2024"
authors:
- admin
date: "2024-11-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2024-07-01T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["paper-conference"]

# Publication name and optional abbreviated publication name.
publication: "IEEE Big Data Conference 2024"
publication_short: "IEEE Big Data 2024"

abstract: "This research paper focuses on improving the data quality of financial time series generative models. By addressing the challenges of synthetic data generation in quantitative finance, this work introduces novel approaches to enhance the fidelity and utility of artificially generated financial time series data for testing, validation, and research purposes."

# Summary. An optional shortened abstract.
summary: "Improving the data quality of financial time series generative models for quantitative finance applications."

tags:
- Big Data
- Generative Models
- Financial Time Series
- Quantitative Finance

featured: true

links:
- name: Preview
  url: http://bit.ly/res-papers
- name: Conference
  url: https://cityuhkfintech.com/2025-conference/
  
# RESOURCE LINKS - Replace '#' with actual URLs or keep as '#' if not applicable
url_pdf: http://bit.ly/res-papers            # LINK TO PDF VERSION
url_code: 'https://github.com/sean-0214/financial-time-series-models'  # LINK TO CODE REPOSITORY
url_dataset: '#'                            # LINK TO DATASET
url_poster: '#'                            # LINK TO RESEARCH POSTER
url_project: '#'                           # LINK TO PROJECT WEBSITE
url_slides: '#'                           # LINK TO PRESENTATION SLIDES
url_source: '#'                           # LINK TO SOURCE DOCUMENT
url_video: '#'                           # LINK TO VIDEO PRESENTATION

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# This image will appear in both the paper list and the paper detail page.
image:
  caption: 'Financial Time Series Generative Models'  # Customize this caption
  focal_point: "Center"  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  preview_only: false  # Show only the image for previews?
  
# IMPORTANT: Place your publication image in this directory and name it 'featured.jpg' or 'featured.png'
# Path: content/publication/ieee-big-data/featured.jpg

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

## Research Overview

This research paper addresses the significant challenges in generating high-quality synthetic financial time series data. Financial markets exhibit unique characteristics—non-stationarity, regime changes, and complex correlations—that make traditional generative models insufficient for creating realistic synthetic data.

## Key Innovations

Our approach introduces several key innovations:

1. **Regime-Aware Generation**: A novel architecture that explicitly models different market regimes (bull, bear, high volatility) and transitions between them
2. **Preservation of Statistical Properties**: Techniques to ensure generated data maintains critical statistical properties of financial time series
3. **Multi-Resolution Temporal Dependencies**: Capturing dependencies across multiple time scales (short-term, medium-term, long-term)
4. **Reality Metrics**: New evaluation metrics specifically designed for financial time series data quality assessment

## Applications

The improved generative models enable:

- More robust backtesting of trading strategies
- Enhanced risk management through more realistic stress testing scenarios
- Better training data for machine learning models in finance
- Privacy-preserving data sharing for collaborative research

## Future Directions

Our ongoing work focuses on incorporating additional market factors and expanding the model to handle multi-asset correlations and alternative data sources.

<!-- Image placeholder -->
<!-- Add a featured.jpg image to this directory for the publication thumbnail -->

<!-- Additional resources -->
<!-- 
To add supplementary materials:
1. Create a "resources" subfolder
2. Add PDF, code samples, or other materials
3. Link to them in the text
-->
