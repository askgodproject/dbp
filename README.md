# Digital Bible Platform (DBP) Library
Python library for accessing the Digital Bible Platform API

## Setup

1. Install Python3 if you don't have it already.
2. Install the Python-Scripture module (`pip3 install python-scriptures`)
- [Reference](https://pypi.org/project/python-scriptures/)
- [Repo](https://github.com/davisd/python-scriptures)

Make sure that the installed package is on the system PATH. If using VSCode, you may need to select a different python interpreter (CMD+SHIFT+P -> python: select interpreter)

3. Obtain Digital Bible Platform API key and set in corresponding environment variable

## Usage

`python3 biblereader.py <passage reference> <language> <version> [<output file>]`

The passage reference should be in the OSIS format.

Examples:
- `python3 biblereader.py John.3.16 ENG ESV`
- `python3 biblereader.py John.3.16-John.3.18 ENG ESV output.txt`

You can retrieve single verses, passages within a chapter, and passages across chapters.

Note that the DPB only has a subset of "text" Bible translations available in English and other languages. They have many "audio / video" Bible reasources, but those aren't used here.

