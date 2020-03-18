# startup-acquisition-tracker
### A of Python scripts that detects if a UK startup has been acquired by a tech giant

This repo contains a set of scripts coded in Python that when used together can detect if a UK startup has been acquired by a tech giant like Apple or Facebook. The scripts match a pre-gathered list of UK startup names, sourced from sites like AngelList and Crunchbase, with new account filings on Companies House via the registrar's API, checking if a tech giant's name or address has appeared, 

It relies on the following Python modules:
- ```requests``` Basic Python module used to use the Companies House API
- ```fuzzywuzzy``` A package for fuzzy matching strings. This is used by the scripts to match startup names with companies returned from the Companies House
- ```pdf2image``` Converts from pdf files to images. Though account filings are uploaded to Companies House in pdf format, the text cannot simply be extracted by a tool like pdfminer because each page of the pdf is an image - presumably because the account filings have just been scanned in (nightmare!). So this package converts the pdf to a collection of images which are then passed to...
- ```pytesseract``` An optical character recognition tool for python. This is used to extract text from the images of account filing pages converted from their pdf form

## How it works

The

1. ```firststage.py```

This 

## Further info

The code is hosted on PythonAnywhere.com.

By Kim Darrah.

