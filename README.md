



## *myprosody package includes all my-voice-analysis' functions plus new functions which you might consider to use instead. The latest myproody update is available here, in Github as well as PYPI, the python library.*  

## NOTE:
    1- Both My-Voice-Analysis and Myprosody work on Python 3.7 
    2- If you install My-Voice-Analysis through PyPi, please use: 
          mysp=__import__("my-voice-analysis") instead of import myspsolution as mysp
    3- It it better to keep the folder names as single entities for instance "Name_Folder" or "NameFolder" without space in the dirctoy path

# my-voice-analysis

My-Voice Analysis is a Python library for the analysis of voice (simultaneous speech, high entropy) without the need of a transcription. It breaks utterances and detects syllable boundaries, fundamental frequency contours, and formants. Its built-in functions recognise and measures 

1.	gender recognition, 
2.	speech mood (semantic analysis), 
3.	pronunciation posterior score 
4.	articulation-rate, 
5.	speech rate,
6.	filler words, 
7.	f0 statistics, 

The library was developed based upon the idea introduced by Nivja DeJong and Ton Wempe [1], Paul Boersma and David Weenink [2], Carlo Gussenhoven [3], S.M Witt and S.J. Young [4] and Yannick Jadoul [5]. Peaks in intensity (dB) that are preceded and followed by dips in intensity are considered as potential syllable cores. 
My-Voice Analysis is unique in its aim to provide a complete quantitative and analytical way to study acoustic features of a speech. Moreover, those features could be analysed further by employing Python’s functionality to provide more fascinating insights into speech patterns. 
This library is for Linguists, scientists, developers, speech and language therapy clinics and researchers.   
Please note that My-Voice Analysis is currently in initial state though in active development. While the amount of functionality that is currently present is not huge, more will be added over the next few months.

## Installation

my-voice-analysis can be installed like any other Python library, using (a recent version of) the Python package manager pip, on Linux, macOS, and Windows:

                                        pip install my-voice-analysis

or, to update your installed version to the latest release:

                                         pip install -u my-voice-analysis



## Development

My-Voice-Analysis was developed by Sab-AI Lab in Japan (previously called Mysolution). It is part of a project to develop Acoustic Models for linguistics in Sab-AI Lab. That is planned to enrich the functionality of My-Voice Analysis by adding more advanced functions as well as adding a language models. Please see Myprosody https://github.com/Shahabks/myprosody and Speech-Rater https://shahabks.github.io/Speech-Rater/)

## Pronunciation
My-Voice-Analysis and MYprosody repos are two capsulated libraries from one of our main projects on speech scoring. The main project (its early version) employed ASR and used the Hidden Markov Model framework to train simple Gaussian acoustic models for each phoneme for each speaker in the given available audio datasets, then calculating all the symmetric K-L divergences for each pair of models for each speaker. What you see in these repos are just an approximate of those model without paying attention to level of accuracy of each phenome rather on fluency 
In the project's machine learning model we considered audio files of speakers who possessed an appropriate degree of pronunciation, either in general or for a specific utterance, word or phoneme, (in effect they had been rated with expert-human graders). Here below the figure illustrates some of the factors that the expert-human grader had considered in rating as an overall score

![image](https://user-images.githubusercontent.com/27753966/98312800-cf583a80-2015-11eb-9ecb-99658ecabdbb.png)

> [S. M. Witt, 2012 “Automatic error detection in pronunciation training: Where we are and where we need to go,” ](https://www.researchgate.net/publication/250306074_Automatic_Error_Detection_in_Pronunciation_Training_Where_we_are_and_where_we_need_to_go)

## References and Acknowledgements

1.	DeJong N.H, and Ton Wempe [2009]; “Praat script to detect syllable nuclei and measure speech rate automatically”; Behavior Research Methods, 41(2).385-390.
2.	 Paul Boersma and David Weenink;  http://www.fon.hum.uva.nl/praat/
3.	Gussenhoven C. [2002]; “ Intonation and Interpretation: Phonetics and Phonology”; Centre for Language Studies, Univerity of Nijmegen, The Netherlands.  
4.	Witt S.M and Young S.J [2000]; “Phone-level pronunciation scoring and assessment or interactive language learning”; Speech Communication, 30 (2000) 95-108.
5.	Jadoul, Y., Thompson, B., & de Boer, B. (2018). Introducing Parselmouth: A Python interface to Praat. Journal of Phonetics,
   71, 1-15. https://doi.org/10.1016/j.wocn.2018.07.001 (https://parselmouth.readthedocs.io/en/latest/)
6. Projects https://parselmouth.readthedocs.io/en/docs/examples.html
7. "Automatic scoring of non-native spontaneous speech in tests of spoken English", Speech Communication, Volume 51, Issue 10, October 2009, Pages 883-895
8. "A three-stage approach to the automated scoring of spontaneous spoken responses", Computer Speech & Language, Volume 25, Issue 2, April 2011, Pages 282-306
9. "Automated Scoring of Nonnative Speech Using the SpeechRaterSM v. 5.0 Engine", ETS research report, Volume 2018, Issue 1, December 2018, Pages: 1-28

 ### MIT License
                                                       
•	Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
•	The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
•	THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.


