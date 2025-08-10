# The Spatial Reasoning Gap in Vision–Language Models

**Understanding Positional Encoding Limitations in Multimodal Models**  
Semester Project — Nayanika Debnath, ETH Computer Science  
Advisors: Yifan Hou · Supervisor: Prof. Mrinmaya Sachan  
Date: August 10, 2025

## Abstract
Modern vision and language models can recognize objects almost perfectly but often fail to reason about spatial relationships. This project evaluates Qwen2-VL-2B on DiagramVQA and on synthetic icon/arrow grids to determine whether spatial errors come from architectural limitations or from poor positional encodings. We measure entity recognition, counting, relation recognition, and localization. Results show strong entity recognition but large failures on spatial relation and counting tasks, suggesting weaknesses in 2D RoPE-based positional embeddings. We also show that patch-based (local) inference can improve some spatial queries.

## Files included
- `image_grid.ipynb` — how synthetic grids are created.
- `masking_analysis.ipynb` — masking experiments (random image regions removed).
- `synthetic_entity.ipynb` — entity counting & localization on synthetic grids.
- `query_analysis.ipynb` — question analysis on DiagramVQA.
- `crop_analysis.ipynb` — patch-only / crop analysis experiments.

## Quick usage
1. Clone the repo and open notebooks in Jupyter / Colab.
2. Outputs were stripped to keep repo small; re-run cells to reproduce figures/outputs.
3. Large datasets / assets are intentionally excluded (see `spatial-aux` on your machine for archived files).

## Contact
Nayanika Debnath — ndebnath@ethz.ch
