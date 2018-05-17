# TWP-wordseg

TWP-wordseg is the word segmentation library of Thai language.

## Installation

To install twp-wordseg you will need:
  1. [Download Python 2.7.x](https://www.python.org/download/releases/2.7/)
  2. [Download Marisa-trie library](https://pypi.python.org/pypi/marisa-trie)
   

### How TWP-wordseg works

We use the forward-maximum length word cut for segmentation to find the longest word in the dictionary and the program will keep searching until there is no any matching in the dictionary.

### How to use TWP-wordseg

To segment the word the user needs to save and copy/import the text file to the input folder then run TWP-wordseg via Python.
After, the process finished the program will create the segmented file which placed in the output folder with the same name as the file in the input folder. 

### 


## The corpus

We use the LEXiTRON Thai words dictionary corpus which developed by NECTEC to reference to our wordsegmentation.

## Built With

* [Python](https://www.python.org) 
* [LEXiTRON](http://lexitron.nectec.or.th)
* [Marisa-trie library](https://pypi.python.org/pypi/marisa-trie)

## Analysis on Error 

There are some of the error in our program
  1.Segmentation that require the context match. Due to the longest matching algorithm our program still facing some of the problem on some of the word such as 'จับตาดูดอกเบี้ย' when we segmented it the output will result as จับ|ตา|ดูด|อก|เบี้ย which the expected output is จับ|ตา|ดู|ดอก|เบี้ย
  2.Lack of words in corpus , no enough words to reference stored in the corpus
  

## Conclusion

In this project, we present a segmentation methodology of Thai words. However, we still faces the errors from many factor that interrupt  the system such as the corpus, the synonym,acronym and aslo the ambiguity of Thai words which is one of the main reason why we can not segment the Thai word from the sentences with 100 percentage accuracy.
Future work might mainly concern on the improvement of the corpus and the special case method that might be assigned with some paring text so, when the programming fing this word it will be send to check the similarity between itself with the corpus.

## Authors
* Ms. Natcha  Sovipa  5822783346 
* Mr. Thanapong  Maleewan  5822790275
* Mr. Dhawin Kritsernvong  5822791026
