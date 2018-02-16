# TWP-wordseg

TWP-wordseg is the word segmentation library of Thai language 

## Installation

To install twp-wordseg you will need:
  1. [Download Python 2.7.x](https://www.python.org/download/releases/2.7/)
  2. [Download Marisa-trie library](https://pypi.python.org/pypi/marisa-trie)
   

### How TWP-wordseg works

We use the forward-maximum length word cut for segmentation to find the longest word in the dictionary and the program will keep searching until there is no any matching in the dictionary.

### How to use TWP-wordseg

To segment the word the user needs to save and copy/import the text file to the input folder then run TWP-wordseg via Python.
After, the process finished the program will create the segmented file which placed in the output folder with the same name as the file in the input folder 

### 


## The corpus

We use the LEXiTRON Thai words dictionary corpus which developed by NECTEC to reference to our wordsegmentation

## Built With

* [Python](https://www.python.org) 
* [LEXiTRON](http://lexitron.nectec.or.th)
* [Marisa-trie library](https://pypi.python.org/pypi/marisa-trie)


## Authors
* Ms. Natcha  Sovipa  5822783346 
* Mr. Thanapong  Maleewan  5822790275
* Mr. Dhawin Kritsernvong  5822791026
