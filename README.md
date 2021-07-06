# doccano_to_bilou
###### Convert Annotation Output (JSONL) From Doccano To Spacy Training Ready BILOU Format.

## Problem
Doccano exports the annotation data in JSONL format which isn't directly supported for spacy training. Doccano does have an official tool for conversion called doccano_transformer but it has a lot of issues and isn't being actively maintained.

## Solution

This script converts the doccano output from JSONL to spacy compatible json in BILOU(Begin, Inside, Last, Unit, Out) format, which is another form of IOB encoding.

#### Steps to use

* 1. Clone The Repo
* 2. Run The Script
```bash
> python convert.py 'file_path'
```

The script will save the output to the same directory by the name <code>annotation_iob.json</code>
