# Huffman and LZW Compression Visualiser on Nigerian Languages

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Eyimofe-y/lzw-huffman-compression/blob/main/huffman_lzw_visualiser.ipynb)
[![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)](https://python.org)

A visual and interactive notebook exploring how two classic compression algorithms perform across **English, Yoruba, Igbo, Hausa, Nigerian Pidgin and random text** and what that reveals about the structure of each language.

---

## What it does

- **Huffman coding**: builds an optimal binary tree for each language based on character frequency. Frequent characters get shorter codes; rare ones get longer codes.
- **LZW compression**: learns repeating patterns as it reads through a text. The faster its dictionary flattens, the more structure (and compressibility) the language has.
- **Shannon entropy**: plots the theoretical minimum bits-per-character for each language, so you can see how close each algorithm gets to the ceiling.

All four outputs are compared side-by-side in an interactive dashboard.

---

## Why Nigerian languages?

English-trained compressors are everywhere. But Yoruba, Igbo and Hausa have different character frequency distributions (different vowel patterns, tonal markers, loanword structures) so a compressor optimised for English will underperform on them.

This matters for Nigerian telecoms systems handling multilingual data at scale. The notebook makes that difference visible.

---

## Visualisations included

| Visual | What it shows |
|---|---|
| Huffman tree (interactive) | The actual binary tree for any input text; switch between languages and watch the shape change |
| LZW dictionary growth chart | How fast each languages patterns are learned. Random text never flattens, structured languages do |
| Compression dashboard | Size saved (%), bits/char and entropy floor across all 6 texts |
| Summary report | Printed metrics table: original size, Huffman savings, LZW savings, gap to Shannon floor |

---

### Option 1 — Google Colab (zero setup)

Click the **Open in Colab** badge at the top of this README to run the simulation in your browser instantly.

### Option 2 — Local installation

```bash
# 1. Clone the repository

# 2. Install dependencies
pip install numpy scipy matplotlib jupyter

# 3. Launch the notebook
jupyter notebook signal_noise_simulator.ipynb
```

---

## Related work

This notebook is part of a broader series exploring information theory and compression through a Nigerian lens, starting from Shannon's probabilistic model and extending into source coding. See also: [signal-noise-simulator](https://github.com/Eyimofe-y/signal-noise-simulator) for the Shannon channel capacity side of the same framework.

---

## License

Distributed under the MIT License. See `LICENSE` for more information.

---

## 🤝 Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://www.linkedin.com/in/oluwaferanmi-eyimofe-yesufu-164b72222/)
