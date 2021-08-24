# Princeton ORF522 Linear and Nonlinear Optimization Companion

[![Binder](http://mybinder.org/badge_logo.svg)](http://mybinder.org/v2/gh/orf522/companion/main?urlpath=lab)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/orf522/companion/blob/main)
[![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.jupyter.org/github/ORF522/companion/tree/main/)

Supporting material for [Princeton ORF307 course: Optimization](https://stellato.io/teaching/orf522)


## Troubleshooting

- `Failed to process string with tex because latex could not be found` when generating plots.
  You most likely do not have latex installed (not present by default in colab). You can simply fix this by commenting the line:

  ```python
  # "text.usetex": True,
  ```
