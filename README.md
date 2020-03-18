# startup-acquisition-tracker
### A of Python scripts that detects if a UK startup has been acquired by a tech giant

This repo contains a set of scripts coded in Python that when used together can detect if a UK startup has been acquired by a tech giant like Apple or Facebook. The scripts match a pre-gathered list of UK startup names, sourced from sites like AngelList and Crunchbase, with listings on Companies House, 

It relies on the following Python modules
- ```fuzzywuzzy``` A package for fuzzy matching strings. This is used by the scripts to match startup names with companies listed on Companies House
- ```pdf2image``` A converter from pdf files to images. Though account filings are uploaded to Companies House, - presumably because the pdf (nightmare!). So this package converts the pdf to a collection of images which are then passed to...
- ```pytesseract``` An optical character recognition tool for python. This is used to extract from the images of account filing pages converted from 

------------------
## How it works

The

1. ```firststage.py```

The code is hosted on PythonAnywhere.com.

