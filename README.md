# Actor-Critic for Sequence Prediction

The reference implementation for the paper

An Actor-Critic Algorithm for Sequence Prediction
([openreview](https://openreview.net/pdf?id=SJDaqqveg), submitted to ICLR 2017)

Note, that in fact it is a heavily modified [speech
recognizer](https://github.com/rizar/attention-lvcsr), so please do not be
surprised by the presense of speech related terms in the code.


### How to use

- install all the dependencies (see the list below)
- set your environment variables by calling `source env.sh`
- for training use `$LVSR/bin/run.py train <save-to> <config>`
- for testing use `$LVSR/bin/run.py search <model-path> <config>`

Please proceed to [`exp/ted`](exp/ted/README.md) for the instructions how
to replicate our machine translation results on TED data, or to 
[`exp/billion_words`](exp/billion_words/README.md)
in order to run our spelling correction experiments.

### Dependencies

- Python packages: pykwalify, toposort, pyyaml, numpy, pandas, picklable-itertools;
- [`blocks`](https://github.com/mila-udem/blocks)
- [`blocks-extras`](https://github.com/mila-udem/blocks-extras)
- [`fuel`](https://github.com/mila-udem/fuel)

The code in this repository is known to work with master branches of the
repositories listed above as of 21.11.2016

### License

MIT
