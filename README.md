# FASEROH — GSoC 2026 Evaluation Task
## Fast Accurate Symbolic Empirical Representation Of Histograms
**Applicant:** Atta ul Asad | COMSATS University Islamabad

## Task
Train seq2seq models (LSTM + Transformer) to learn 4th-order 
Taylor expansions of mathematical functions using prefix notation.

## Results

| Metric | LSTM | Transformer |
|--------|------|-------------|
| Token Accuracy | 99.50% | 97.94% |
| Sequence Accuracy | 26.67% | 76.67% |
| BLEU Score | 0.5901 | 0.8980 |
| Perplexity | 1.02 | 1.06 |

## Key Finding
Transformer outperforms LSTM on sequence-level accuracy by 3x (76.67% vs 26.67%).
Remaining errors are limited to rational coefficient precision in high-order terms.

## Setup
pip install sympy torch nltk

## Dataset
5000 (function, Taylor expansion) pairs generated with SymPy.
Tokenized using prefix notation (as in Lample & Charton, 2019).

## Reference
Lample, G., & Charton, F. (2019). Deep Learning for Symbolic Mathematics.
