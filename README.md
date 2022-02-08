# A Dataset of French Late Modern Directories

This dataset is composed of pages and entries extracted from late modern French directories (XXXX-YYYY).

It is intended to evaluate the performance of Optical Character Recognition (OCR) 
and Named Entity Recognition (NER) on early late modern, French documents.

TODO entry illustration + text illustration + entities (more than 1)

## How to cite this dataset

Authors (alphabetic order):
Nathalie Abadie
Stéphane Baciocchi
Edwin Carlinet
Joseph Chazalon
Pascal Cristofoli
Bertrand Duménieu
Julien Perret


TODO proper ref

TODO DAS paper ref

## Content and files
TODO summary of resulting content

### Unsupervised Dataset
text of ~7000 pages OCRed with PERO OCR.

TODO files and file formats?


### Supervised dataset
- full-page images (deskewed)
- bounding boxes of entries
- images cropped from bounding boxes???
- human transcription of entries
- human entity tagging of transcriptions
- automated transcription of entries using 3 OCR engines: Tesseract v4, PERO OCR and Kraken
- automated projection of human entity tagging on all OCR predictions (when possible)


WARNING check/remove bad bounding boxes


Named entities:
- TODO list (from paper)


TODO files and file formats?


About the OCR systems:
TODO (cite or copy paper)


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
???


## Version and revisions
useful? probably if we have more than 1 upload

