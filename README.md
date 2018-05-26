# TWP_Word-Seg



## Overview : TWP_Word-Seg
TWP_Word-Seg is the word segmentation software for Thai language. 
This software consists of :
 
 - backtrack.py as the word segmentation 
 - Input folder : Where users insert the text files that they want to segment into.
 - Output folder : Where users received the segmented files that they put the original files in the Input Folder.
 

## PART1. Installation

To use TWP_Word-Seg you will need:
  
  1. [Download Python 2.7.x](https://www.python.org/download/releases/2.7/)
  2. [Download Marisa-trie library](https://pypi.python.org/pypi/marisa-trie)
  


### 1.1 Installing Python Version 2.7.x and  Marisa-trie library
### 1.2 Run backtrack.py via Python IDE


## PART2. Algorithms

Our software consist of 2 algorithms inside respectively from executing task which are :
  
  1. Longest Matching to select the longest word and compare the word with the corpus.
  2. Back Track Matching to correct the word again in case that when we use the Longest Matching then we matched that first but the sencond word has no meaning left
      eg. Original sentence = ' เมื่อยามน้ัน' the expected cut sentence is 'เมื่อ|ยาม|นั้น  but the result is 'เมื่อย|าม|นั้น'.

## PART3. How to use TWP_Word-Seg
There 2 ways of using our software :

  1. By sentence directly via Python IDE : segmentSentence() you can fill the string of the sentence that you want to segment.
        ![alt text](http://git.vssiit.xyz/css432-y18s2/TWP_Word-Seg/raw/master/referencepicture/pic1.jpg)

  2. By choosing the input directory by typinging its path file to Python  IDE: segmentFolder() if you did not fill the path file of input, the default is input folder at the same directory of your python file.<br>
        ![alt text](http://git.vssiit.xyz/css432-y18s2/TWP_Word-Seg/raw/master/referencepicture/pic2.jpg)

## PART4. Analysis on the Errors

There are some of the error in our program :
  1. Segmentation that require the context match. Due to the longest matching algorithm our program.
  2. Lack of words in corpus,not enough words to reference stored in the corpus.
   

## PART5. The Corpus

We use the LEXiTRON Thai words dictionary corpus which developed by NECTEC to reference to our wordsegmentation.

## PART6. Conclusion and Further Implementation

In this project, we present a segmentation methodology of Thai words. However, we still faces some errors from many factors that interrupt the system.
  1. The corpus which the number of words that covers might not enough.
  2. The synonym, acronym and also the ambiguity in context of Thai words that some subject composes of 'N'+'V' to be 1 word which is one of the main reason why we can not segment the Thai word from the sentences with 100 percentage accuracy.<br>

For the future work might mainly concern on the improvement of the corpus and the special case method that might be assigned with some paring text so, when the programming find this word it will be send to check the similarity between itself with the corpus.

## Built With

* [Python](https://www.python.org) 
* [LEXiTRON](http://lexitron.nectec.or.th)
* [Marisa-trie library](https://pypi.python.org/pypi/marisa-trie)

---
This word segmentation library is a part of CSS432 Information Retrieval submitted to Dr.Virach Sornlertlamvanich.
## Authors
* Ms. Natcha  Sovipa  5822783346 
* Mr. Thanapong  Maleewan  5822790275
* Mr. Dhawin Kritsernvong  5822791026
