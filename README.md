# A Dataset of French Trade Directories from the 19th Century (FTD)

This dataset is composed of pages and entries extracted from late modern French directories (1798-1861).

It is intended to evaluate the performance of Optical Character Recognition (OCR) 
and Named Entity Recognition (NER) on French documents produced between 1789 and 1950.

TODO entry illustration + text illustration + entities (more than 1)


## How to cite this dataset
Please cite this dataset as:
```
N. Abadie, S. Baciocchi, E. Carlinet, J. Chazalon, P. Cristofoli, B. Duménieu and J. Perret, A Dataset of French Trade Directories from the 19th Century (FTD), version 1.0.0, March 2022, online at https://doi.org/10.5281/zenodo.6394464.
```

```bibtex
@dataset{abadie_dataset_22,
  author       = {Abadie, Nathalie and
                  Bacciochi, St{\'e}phane and
                  Carlinet, Edwin and
                  Chazalon, Joseph and
                  Cristofoli, Pascal and
                  Dum{\'e}nieu, Bertrand and
                  Perret, Julien},
  title        = {{A} {D}ataset of {F}rench {T}rade {D}irectories from the 19th {C}entury ({FTD})},
  month        = mar,
  year         = 2022,
  publisher    = {Zenodo},
  version      = {v1.0.0},
  doi          = {10.5281/zenodo.6394464},
  url          = {https://doi.org/10.5281/zenodo.6394464}
}
```

You may also be interested in our paper accepted at DAS 2022 (15th IAPR International Workshop on Document Analysis Systems), which compares the performance of OCR and NER systems on this dataset:

```
N. Abadie, E. Carlinet, J. Chazalon and B. Duménieu, A Benchmark of Named Entity Recognition Approaches in Historical Documents — Application to 19th Century French Directories, May 2022, La Rochelle, France, Springer.
```

```bibtex
@inproceedings{abadie_das_22,
  author       = {Abadie, Nathalie and
                  Carlinet, Edwin and
                  Chazalon, Joseph and
                  Dum{\'e}nieu, Bertrand},
  title        = {{A} {B}enchmark of {N}amed {E}ntity {R}ecognition {A}pproaches in {H}istorical {D}ocuments — {A}pplication to 19th {C}entury {F}rench {D}irectories},
  month        = may,
  year         = 2022,
  publisher    = {Springer},
  place        = {La Rochelle, France}
}
```

## Content and files
The dataset we provide is divided into two sub-parts:

1. A **labeled dataset**, 
   which contains 8765 manually corrected entries from 78 pages (18 different directories), 
   and which is designed for *supervised training*.
2. An **unlabeled dataset**,
   containing 1058196 raw entries from 6887 pages (13 different directories), 
   and which is designed for *unsupervised pre-training*.


TODO content summary

FIXME WIP ~/work/datasets/french_trade_directories_19th_century


### Labeled dataset (for supervised training and evaluation)
- [x] full-page images (deskewed)
- [x] bounding boxes of entries
- [x] images cropped from bounding boxes???
- [x] human transcription of entries
- [x] human entity tagging of transcriptions
- automated transcription of entries using 3 OCR engines: Tesseract v4, PERO OCR and Kraken
- automated projection of human entity tagging on all OCR predictions (when possible)

(pretty OK)


Named entities:
- TODO list (from paper)


TODO files and file formats?


About the OCR systems:
TODO (cite or copy paper)


Directories:
"Bottin1_1820"
"Bottin1_1827"
"Bottin1_1837"
"Bottin3_1854a"
"Cambon_almgene_1841"
"Deflandre_1828"
"Deflandre_1829"
"Didot_1841a"
"Didot_1851a"
"Didot_1854a"
"DidotBottin_1860a"
"DidotBottin_1861a"
"Duverneuil_et_La_Tynna_1801"
"Duverneuil_et_La_Tynna_1805"
"Duverneuil_et_La_Tynna_1806"
"Favre_et_Duchesne_1798"
"La_Tynna_1813"
"Notables_communaux_seine_1801"


### Labeled dataset (for unsupervised pre-training)
text of ~7000 pages OCRed with PERO OCR.

TODO files and file formats?

Directories:
"Bottin1_1827"
"Bottin1_1837"
"Bottin3_1854a"
"Cambon_almgene_1841"
"Deflandre_1828"
"Didot_1841a"
"Didot_1851a"
"Didot_1854a"
"DidotBottin_1860a"
"DidotBottin_1861a"
"Duverneuil_et_La_Tynna_1805"
"Favre_et_Duchesne_1798"
"La_Tynna_1813"


## How this dataset was created

### Original documents

TODO Gallica and other ref

### Selection of relevant pages
present listings

TODO table of relevant pages

### Sampling process
Pages were randomly sampled from relevant sections.

TODO Table of selected pages

### Annotation process
image dewarping
automatic processing
manual inspection and correction

### Quality assessment of human annotations
NONE -- do it for full-length paper?


## Copyright
The images were extracted from the original source https://gallica.bnf.fr, owned by the Bibliothèque nationale de France (French national library).
Original contents from the Bibliothèque nationale de France can be reused non-commercially, provided the mention "Source gallica.bnf.fr / Bibliothèque nationale de France" is kept.
Researchers do not have to pay any fee for reusing the original contents in research publications or academic works.
Original copyright mentions extracted from https://gallica.bnf.fr/edit/und/conditions-dutilisation-des-contenus-de-gallica on March 29, 2022.

The original contents were significantly transformed before being included in this dataset.
All derived content is licensed under the permissive *Creative Commons Attribution 4.0 International* license.

## Version and semantics
Current dataset version is `1.0.0`.

We try to adhere to [Semantic Versioning 2.0.0](https://semver.org/) despite the precise meaning for datasets is unclear.
Here are the rules we will follow, if necessary.

Given a version number MAJOR.MINOR.PATCH, we will increment the:

- MAJOR version when we make incompatible evaluation changes (add, remove, change data),
- MINOR version when we add functionality (like an export in a new archive format) in a backwards compatible manner, and
- PATCH version when we make backwards compatible bug fixes (like documentation fixes).

### Revisions
- `1.0.0` - 2022-04-01 - Initial release.

