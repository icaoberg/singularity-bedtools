# singularity-bedtools
[![Hosted](https://img.shields.io/badge/hosted-sylabs.io-green.svg)](https://cloud.sylabs.io/library/icaoberg/default/bedtools)
![Release](https://img.shields.io/badge/release-v2.29.2-green.svg)
[![Build Status](https://travis-ci.org/icaoberg/singularity-bedtools.svg?branch=master)](https://travis-ci.org/icaoberg/singularity-bedtools)
[![GitHub issues](https://img.shields.io/github/issues/icaoberg/singularity-bedtools.svg)](https://github.com/icaoberg/singularity-bedtools/issues)
[![GitHub forks](https://img.shields.io/github/forks/icaoberg/singularity-bedtools.svg)](https://github.com/icaoberg/singularity-bedtools/network)
[![GitHub stars](https://img.shields.io/github/stars/icaoberg/singularity-bedtools.svg)](https://github.com/icaoberg/singularity-bedtools/stargazers)
[![GitHub license](https://img.shields.io/badge/license-GPLv3-blue.svg)](https://www.gnu.org/licenses/quick-guide-gplv3.en.html)

![Logo](images/logo.png)

Collectively, the [bedtools](https://bedtools.readthedocs.io/en/latest/) utilities are a swiss-army knife of tools for a wide-range of genomics analysis tasks. The most widely-used tools enable genome arithmetic: that is, set theory on the genome. For example, bedtools allows one to intersect, merge, count, complement, and shuffle genomic intervals from multiple files in widely-used genomic file formats such as BAM, BED, GFF/GTF, VCF. While each individual tool is designed to do a relatively simple task (e.g., intersect two interval files), quite sophisticated analyses can be conducted by combining multiple bedtools operations on the UNIX command line.

## Pre-requisites

* [Singularity v3.5.+](https://sylabs.io/docs/).

## Building the image using the recipe

### To build the image locally
Run the script `build.sh` to build image locally.

```
bash ./build.sh
```

### To build the image remotely remotely
Run the script `rbuild.sh` to build image remotely.

```
bash ./rbuild.sh
```

You will need to edit the script above to match your account on [SyLabs.io](https://sylabs.io/).

### Pulling from the repository
If you have the client installed and cannot build the image locally nor remotely, simply run

```
singularity pull --arch amd64 library://icaoberg/default/bedtools:v2.29.2
```

## Disclaimer

I am nothing but a humble programmer creating the container for this wonderful app. [bedtools](https://bedtools.readthedocs.io/en/latest/) is developed in the [Quinlan laboratory](http://quinlanlab.org/) at the [University of Utah](https://www.utah.edu/) and benefits from fantastic contributions made by scientists worldwide.

---
[![CBD](http://www.cbd.cmu.edu/wp-content/uploads/2017/07/wordpress-default.png)](http://www.cbd.cmu.edu)

Copyleft © 2019-2020 [icaoberg](http://www.andrew.cmu.edu/~icaoberg) at the [Computational Biology Department](http://www.cbd.cmu.edu) in [Carnegie Mellon University](http://www.cmu.edu)
