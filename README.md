# ACR-Chord-Recognition
Automatic Chord Recognition with Data Augmentation



# Improving Chord Recognition Through
# Noise and Distortion Augmentation

**Authors:** Manish Bandi,
Douglas W. Cunningham,
Prashant Varadarajan
BTU Cottbus-Senftenberg, Germany

---

## Overview
Reimplementation and extension of
Korzeniowski & Widmer (2016) ACR paper.
Extends baseline CNN with Gaussian noise,
clipping distortion and sample rate
reduction augmentation techniques.
Evaluated using WCSR with mir_eval
on Isophonics Beatles dataset.

---

## Requirements
pip install -r requirements.txt

---

## Dataset
Download Isophonics Beatles dataset
from isophonics.net
Place in: Originals/TheBeatles/

---

## How to Run
1. Upload project to Google Drive
2. Open ACR_Main.ipynb in Google Colab
3. Enable GPU runtime
4. Run Data-Augmentation.ipynb first
5. Run ACR_Main.ipynb cells in order

---

## Results

| Condition  | Baseline | Augmented |
|------------|----------|-----------|
| Original   | 55.5%    | 58.8%     |
| Noisy      | 55.3%    | 59.0%     |
| Distorted  | 56.6%    | 60.0%     |
| Quality    | 54.7%    | 59.1%     |

Augmented model outperforms baseline
on ALL conditions (+3.7% avg WCSR)

---

## Reference
Korzeniowski & Widmer (2016)
IEEE MLSP, Salerno, Italy
