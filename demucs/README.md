# Demucs hybrid transformer weights

Unmodified copies of the pretrained [Demucs](https://github.com/facebookresearch/demucs) v4 hybrid transformer weights from Meta. Cleave uses them to split a song into stems. Cleave uses `htdemucs` for a standard separate and `htdemucs_ft` (a bag of four fine-tuned models) for a High quality separate.

Release tag: `demucs-v1`. All five files are attached to that one release, under their upstream names.

| Model | File | Size (bytes) | SHA-256 |
| --- | --- | --- | --- |
| `htdemucs` | `955717e8-8726e21a.th` | 84,141,911 | `8726e21a993978c7ba086d3872e7608d7d5bfca646ca4aca459ffda844faa8b4` |
| `htdemucs_ft` | `f7e0c4bc-ba3fe64a.th` | 84,141,271 | `ba3fe64ae8ef66ac9a4857222ce48efbdc5eb3ad375cb79dd13debee5aaa4066` |
| `htdemucs_ft` | `d12395a8-e57c48e6.th` | 84,141,271 | `e57c48e6b0e38af4f7118d7bd08c49f0a0c0edf7d09143bdd902ea0d237303e6` |
| `htdemucs_ft` | `92cfc3b6-ef3bcb9c.th` | 84,141,271 | `ef3bcb9c8b40d14ae5d51b6db2587339cc12c6b77c0be151ce6d69002e087bf2` |
| `htdemucs_ft` | `04573f0d-f3cf25b2.th` | 84,141,271 | `f3cf25b222c4eed7cd49dd8b2c9597d50c18bd154090f7b919cfa5f93cf22c49` |

The second half of each file name is the start of its SHA-256. Torch hub checks it on download.

Upstream: `https://dl.fbaipublicfiles.com/demucs/hybrid_transformer/<file>`, as listed in `demucs/remote/files.txt` of the `demucs` 4.0.1 package. The upstream repository was archived on 1 January 2025; development continues at [adefossez/demucs](https://github.com/adefossez/demucs).

## License

Demucs is released under the MIT license, with no separate terms for its pretrained weights. The copyright notice and permission notice in [LICENSE](LICENSE) are reproduced exactly from the upstream repository. If the copyright holder asks for these files to be removed, they will be.

Download, for example:

```
https://github.com/SpoddyCoder/cleave-resources/releases/download/demucs-v1/955717e8-8726e21a.th
```

If you use Demucs in research, cite the authors' papers: Simon Rouard, Francisco Massa, and Alexandre Défossez, "Hybrid Transformers for Music Source Separation", ICASSP 2023; and Alexandre Défossez, "Hybrid Spectrogram and Waveform Source Separation", Proceedings of the ISMIR 2021 Workshop on Music Source Separation. BibTeX is in the [upstream README](https://github.com/facebookresearch/demucs#how-to-cite).
