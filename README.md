Hasnain-2025-QNM-Magnetic-Kiselev/          (main folder)
│
├── README.md                                (description + instructions)
├── LICENSE                                  (MIT, GPL, or CC-BY)
├── CITATION.cff                             (how to cite your paper)
├── requirements.txt                          (Python dependencies)
│
├── code/                                     (all analysis scripts)
│   ├── figure1_f_of_r.py                      (metric function plots)
│   ├── figure2_V_eff.py                       (effective potential)
│   ├── figure3_rstar.py                       (tortoise coordinate)
│   ├── figure4_waveform.py                    (time-domain evolution)
│   ├── figure5_Q_results.py                    (Q vs frequency plots)
│   ├── figure6_c_results.py                    (c vs frequency plots)
│   ├── wkb_qnm.py                             (WKB frequency calculator)
│   ├── timedomain.py                          (time-domain integrator)
│   └── prony_fit.py                           (Prony extraction)
│
├── data/                                      (optional: pre-computed tables)
│   └── frequencies_table.txt                   (your numerical results)
│
└── paper/                                     (optional: LaTeX source)
    └── manuscript.pdf                          (for reference)



## About
This repository contains the numerical codes used in the paper:
**"Scalar quasinormal modes of a magnetically charged Kiselev black hole"** by Ali Hasnain (2026).

We compute scalar quasinormal mode frequencies using:
- Sixth-order WKB approximation
- Time-domain integration with Prony extraction

##  Quick Start

### 1. Clone the repository
```bash
git clone https://github.com/username/Hasnain-2025-QNM-Magnetic-Kiselev.git
cd Hasnain-2025-QNM-Magnetic-Kiselev

python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
pip install -r requirements.txt

python code/figure1_f_of_r.py     # Metric function
python code/figure2_V_eff.py      # Effective potential
python code/figure3_rstar.py      # Tortoise coordinate
python code/figure4_waveform.py   # Time-domain waveform

python code/wkb_qnm.py --Q 0.5 --c 0.05 --omega -0.6667






