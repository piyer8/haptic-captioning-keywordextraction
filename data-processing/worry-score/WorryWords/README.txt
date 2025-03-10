
THE NRC WORRYWORDS LEXICON (aka The NRC Word--Anxiety Association Lexicon)
--------------------------------------------------------------------------

Version:	1
Released: 	October 2024
Copyright: 	2024 National Research Council Canada (NRC)
Created By: Saif M. Mohammad (Principal Research Scientist, National Research Council Canada)

Readme Last Updated: October 2024
Automatic translations from English to 108 languages was last updated: October 2024

Home Page: 	http://saifmohammad.com/WebPages/worrywords.html

Contact: 	Dr. Saif M. Mohammad 
		 	saif.mohammad@nrc-cnrc.gc.ca 
		 	uvgotsaif@gmail.com

TABLE OF CONTENTS

            I.    General Description
            II.   Papers And Citation
            III.  Python Code To Analyze Emotions In Text
            IV.   NRC Emotion Lexicon In Various Languages (will be available in November 2024)
            V.    Lemmatization And Other Techniques That May Be Beneficial
            VI.   Forms Of The Lexicon, Files, And Format
            VII.  Version Information And Change Log
            VIII. Other Emotion Lexicons
            IX.   Terms Of Use
            X.    Ethical Considerations


I. GENERAL DESCRIPTION
----------------------

The NRC WorryWords Lexicon is a list of over 44,000 English words and real-valued scores
indicating their associations with anxiety. The scores were obtained from manual 
annotations through crowdsourcing.

This work was approved by the NRC Research Ethics Board (NRC-REB).  REB review seeks to
ensure that research projects involving humans as participants meet Canadian standards of
ethics.

Companion lexicons -- the NRC Emotion Lexicon and the NRC VAD Lexicon are available here:
http://saifmohammad.com/WebPages/lexicons.html

Applications: The lexicon has a broad range of applications in Computational Linguistics,
Psychology, Digital Humanities, Computational Social Sciences, and beyond. Notably it can
be used for:

-  Understanding anxiety and the underlying mechanisms; how anxiety relates to other
emotions; how it relates to our body; how anxiety changes with age, socio-economic status,
weather, green spaces, etc. 

- Determining how anxiety manifests in language; how language shapes anxiety; how culture
shapes the language of anxiety; etc.

- Tracking the degree of anxiety towards targets of interest such as climate change,
government policies, biological vectors, etc. 

- Identifying effective coping mechanisms and clinical interventions to manage anxiety.

- Developing automatic systems for detecting anxiety; developing chat systems that are
sensitive to nuances and diverse expressions of anxiety by people from various
demographics.

- Studying anxiety and uneasiness in story telling; its relationship with central elements
of narratology such as conflict and resilience.

- Studying how anxiety impacts social behaviour in physical and virtual environments.


II. PAPERS AND CITATION 
-----------------------

- WorryWords: Norms of Anxiety Association for over 44k English Words. Saif M. Mohammad. In
Proceedings of the Empirical Methods on Natural Language Processing (EMNLP 2024, Main),
November 2024, Miami, FL. 

- Saif M. Mohammad. 2024b. Worrywords: A massive lexicon of anxiety associations for
English words and phrases. In ArXiv.

If you use the lexicon in your work, then:

- Cite the papers:
		@inproceedings{worrywords-emnlp24,
    		title = {Worry{W}ords: Norms of Anxiety Association for over 44k {E}nglish Words},
    		author = {Mohammad, Saif M.},
    		booktitle = {Proceedings of the 2024 Conference on Empirical Methods in Natural Language Processing},
    		year = {2024},
    		address = {Miami, FL},
    		publisher = {Association for Computational Linguistics}
		}

		@inproceedings{ww-2,
  			title={WorryWords: A Massive Lexicon of Anxiety Associations for {E}nglish Words and Phrases},
  			author={Mohammad, Saif M.},
    		booktitle={ArXiv},
   	 		year={2024}
		}

- Point to the lexicon homepage: 
		http://saifmohammad.com/WebPages/worrywords.html

Other relevant papers:

- Best Practices in the Creation and Use of Emotion Lexicons.
  Saif M. Mohammad. Findings of the Association for Computational Linguistics: EACL 2023. 2023.

- Ethics Sheet for Automatic Emotion Recognition and Sentiment Analysis.
  Saif M. Mohammad. Computational Linguistics. 48 (2): 239–278. June 2022.


III. PYTHON CODE TO ANALYZE EMOTIONS IN TEXT
--------------------------------------------

There are many third party software packages that can be used in conjunction with the NRC
Emotion Lexicon to analyze emotion word use in text. We recommend Emotion Dynamics:

	https://github.com/Priya22/EmotionDynamics

It is the primary package that we use to analyze text using the NRC Emotion Lexicon and
the NRC VAD Lexicon.  It can be used to generate a csv file with a number of emotion
features pertaining to the text of interest, including metrics of utterance emotion
dynamics. 

See this paper for an example of the use of the lexicon to analyze emotions in text:

	Tweet Emotion Dynamics: Emotion Word Usage in Tweets from US and Canada. Krishnapriya
	Vishnubhotla and Saif M. Mohammad. In Proceedings of the 13th Language Resources and
	Evaluation Conference (LREC-2022), May 2022, Marseille, France.

	https://arxiv.org/pdf/2204.04862.pdf


IV. NRC WORRYWORDS LEXICON IN VARIOUS LANGUAGES (to come in November 2024)
-----------------------------------------------

The NRC WorryWords Lexicon has anxiety annotations for English words. Despite some cultural
differences, it has been shown that a majority of emotional norms are stable across
languages. Thus, we provide versions of the lexicon in over 100 languages by translating
the English terms using Google Translate (November 2024).

The lexicon is thus available for English and these languages:

Afrikaans, Albanian, Amharic, Arabic, Armenian, Azerbaijani, Basque, Belarusian, Bengali,
Bosnian, Bulgarian, Burmese, Catalan, Cebuano, Chichewa, Corsican, Croatian, Czech,
Danish, Dutch, Esperanto, Estonian, Filipino, Finnish, French, Frisian, Gaelic, Galician,
Georgian, German, Greek, Gujarati, HaitianCreole, Hausa, Hawaiian, Hebrew, Hindi, Hmong,
Hungarian, Icelandic, Igbo, Indonesian, Irish, Italian, Japanese, Javanese, Kannada,
Kazakh, Khmer, Kinyarwanda, Korean, Kurmanji, Kyrgyz, Lao, Latin, Latvian, Lithuanian,
Luxembourgish, Macedonian, Malagasy, Malay, Malayalam, Maltese, Maori, Marathi, Mongolian,
Nepali, Norwegian, Odia, Pashto, Persian, Polish, Portuguese, Punjabi, Romanian, Russian,
Samoan, Sanskrit, Serbian, Sesotho, Shona, Simplified, Sindhi, Sinhala, Slovak, Slovenian,
Somali, Spanish, Sundanese, Swahili, Swedish, Tajik, Tamil, Tatar, Telugu, Thai,
Traditional, Turkish, Turkmen, Ukranian, Urdu, Uyghur, Uzbek, Vietnamese, Welsh, Xhosa,
Yiddish, Yoruba, Zulu

Note some of the translations may be incorrect or they may simply be transliterations of 
the original English terms.


V. LEMMATIZATION AND OTHER TECHNIQUES THAT MAY BE BENEFICIAL
------------------------------------------------------------

The lexicon file can be used as is, but occasionally certain additional techniques can be
applied to make the most of it for one's specific application context.

1. LEMMATIZATION: The lexicon largely includes the base forms or lemmas of words. For
example, it may include an entry for 'attack', but not for 'attacks' or 'attacking'. In
many cases, such morphological variants are expected to have similar emotion scores. So
one can first apply a third-party lemmatizer on the target text to determine the base forms
before applying the lexicon. Note that lemmatization must be applied with care; for
example, while it it good to go from 'helplessness' to 'helpless' (they are expected to
have similar emotional connotations), 'helplessness' should not be lemmatized to 'help'
(they are expected to have markedly different emotional connotations). Further, various
factors such as tense and 'differing predominant senses for different morphological forms'
can impact emotionality. So benefits of lemmatization are limited, especially when
analyzing large pieces of text.

2. OTHER: Other techniques such discarding highly ambiguous terms (terms with many
meanings), or identifying most common terms in one's text and inspecting emotion entries
in the lexicon for those terms (and correcting entries where appropriate), etc. are also
good practice.


VI. FORMS OF THE LEXICON, FILES, AND FORMAT 
-------------------------------------------

1. worrywords-v1.txt: This is the primary lexicon file. 

Each line has the following format:
Term<tab>Mean<tab>MajorityLabel<tab>MajorityLabelRatio<tab>NumberAnnotations<tab>SetOfLabels

Term: a word or phrase for which the anxiety association is provided.

Mean: real-valued score indicating the degree of anxiety association. It can range from
      -3 (maximum calmness) to 3 (maximum anxiety).
      It is the average of the anxiety scores provided by the annotators.

OrdinalClass: A discrete class assigned to the word based on the mean.
      The class is one of the following:
             3: very anxious (when mean >= 2.5)
             2: moderately anxious (when mean >= 1.5 and < 2.5)
             1: slightly anxious (when mean >= 0.5 and < 1.5) 
             0: not associated with feeling anxious or calm (when mean > -0.5 and < 0.5) 
            -1: slightly calm (when mean > -1.5 and <= -0.5)
            -2: moderately calm (when mean > -2.5 and <= -1.5)
            -3: very calm (when mean <= -2.5)

MajorityLabel: This is the most common discrete label provided by the annotators.
      The label is one of the following:
			 3: very anxious  
			 2: moderately anxious   
			 1: slightly anxious   
			 0: not associated with feeling anxious or calm
			-1: slightly calm
			-2: moderately calm
			-3: very calm
      We do not recommend using this label. It is provided just for information.
      Instead use either the mean or ordinalClass.

MajorityLabelRatio: Ratio of the number of annotators that provided the majority label to
      the total number of annotators that provided a response for the term.

NumberAnnotations: the total number of annotators that provided a response for the term.

SetOfLabels: A comma-separated list of the individual responses provided by the annotators.


2. Supplementary: This directory has additional supplementary data files.
      It curently includes the file highvariance-anxiety-annotations.txt which has a list of 500+
      terms not included in the main worrywords file, because there was considerable variance in
      their annotations. The file has the same format as worrywords-v1.txt.
      High variance can occur due to many reasons:
      -- not all words fit neatly in the calmness--anxiety dimension;
      -- different senses of a word may be associated with very different degrees of anxiety;
      -- occasional poor annotation; etc.
      It is generally tricky to use these entries; and often the main worrywords file should be 
      sufficient for most aggregate-level text analyses. However, entries from the highvariance
      file may also useful at times; best to exercise caution when using them.

3. Paper-Main-WorryWords.pdf: The research paper describing the NRC WorryWords Lexicon.

4. Paper-Ethics - Best Practices in the Creation and Use of Emotion Lexicons.pdf: Paper listing
practical and ethical considerations in the use of emotion and sentiment lexicons.

5. Paper-Ethics-Sheet-Emotion-Recognition.pdf: Paper discussing ethical considerations involved
in automatic emotion recognition and sentiment analysis.


ENCODING: The lexicon files were created using UTF-8 encoding. You can view the lexicon files using
most text editors, Microsoft Excel, etc. You might have to make sure that the viewer
supports characters from various languages, i.e., set the encoding option in the viewer to
UTF-8, etc.  For example, to view in excel, follow these steps:

- open excel
- click on File -> Import
- select file type as 'Text file'
- select the lexicon file to import in the dialog box that opens up
- select 'File Origin' type as 'Unicode (UTF-8)'
- click 'Finish'


VII. VERSION INFORMATION AND CHANGE LOG
----------------------------------------

- Version 1 is the latest version (Released October 2024).  
- The automatic translations generated using Google Translate are updated every few years.  
  They were last obtained in August 2022. 


VIII. OTHER EMOTION LEXICONS
----------------------------

- The NRC Emotion Intensity Lexicon is a list of English words (taken from the NRC Emotion
Lexicon and other sources) with real-valued scores of intensity for eight discrete emotions
(anger, anticipation, disgust, fear, joy, sadness, surprise, and trust). 

	Word Affect Intensities. Saif M. Mohammad. In Proceedings of the 11th Edition of the Language 
    Resources and Evaluation Conference (LREC-2018), May 2018, Miyazaki, Japan.
    
    http://saifmohammad.com/WebPages/AffectIntensity.htm

- The NRC Valence, Arousal, and Dominance (VAD) Lexicon includes a list of more than 20,000 English words and
their valence, arousal, and dominance scores.  For a given word and a dimension (V/A/D), the scores range from
0 (lowest V/A/D) to 1 (highest V/A/D).

    Obtaining Reliable Human Ratings of Valence, Arousal, and Dominance for 20,000 English Words.  Saif M.
    Mohammad. In Proceedings of the 56th Annual Meeting of the Association for Computational Linguistics,
    Melbourne, Australia, July 2018.

	http://saifmohammad.com/WebPages/nrc-vad.html

Various other emotion lexicons can be found here:
http://saifmohammad.com/WebPages/lexicons.html

You may also be interested in some of the other resources and work we have done on the
analysis of emotions in text:

http://saifmohammad.com/WebPages/ResearchAreas.html
http://saifmohammad.com/WebPages/ResearchInterests.html#EmotionAnalysis


IX. TERMS OF USE 
----------------

1. Research Use: The lexicon mentioned in this page can be used freely for non-commercial
research and educational purposes.

2. Citation: Cite the papers associated with the lexicon in your research papers and
articles that make use of them. 

3. Media Mentions: In news articles and online posts on work using the lexicon, cite the
lexicon. For example: "We make use of the <resource name>, created by <author(s)> at the
National Research Council Canada." We would appreciate a hyperlink to the lexicon home
page and an email to the contact author (saif.mohammad@nrc-cnrc.gc.ca).  (Authors and
homepage information provided at the top of the README.)

4. Credit: If you use the lexicon in a product or application, then acknowledge this in
the 'About' page and other relevant documentation of the application by stating the name
of the resource, the authors, and NRC. For example: "This application/product/tool makes
use of the <resource name>, created by <author(s)> at the National Research Council
Canada." We would appreciate a hyperlink to the lexicon home page and an email to the
contact author (saif.mohammad@nrc-cnrc.gc.ca).

5. NO REDISTRIBUTION: Do not redistribute the data. Direct interested parties to the
lexicon home page.  You may not rent or license the use of the lexicon nor otherwise
permit third parties to use it. Do not upload the lexicon on a public website.

** Important **
Do not upload or store the lexicon in any location that can be scanned by companies or
other entities to create large language models. for example, do not upload to a public
website, Hugging Face, GitHub, etc. 

6. Proprietary Notice: You will ensure that any copyright notices, trademarks or other
proprietary right notices placed by NRC on the lexicon remains in evidence.

7. Title: All intellectual property rights in and to the lexicon shall remain the property
of NRC. All proprietary interests, rights, unencumbered titles, copyrights, or other
Intellectual Property Rights in the lexicon and all copies thereof remain at all times
with NRC.

8. Commercial License: If interested in commercial use of the lexicon, contact the author:
saif.mohammad@nrc-cnrc.gc.ca

9. Disclaimer: National Research Council Canada (NRC) disclaims any responsibility for the
use of the lexicon and does not provide technical support. NRC makes no representation and
gives no warranty of any kind with respect to the accuracy, usefulness, novelty,
validity, scope, or completeness of the lexicon and expressly disclaims any implied
warranty of merchantability or fitness for a particular purpose of the lexicon.  That
said, the contact listed above welcomes queries and clarifications.

10 Limitation of Liability: You will not make claims of any kind whatsoever upon or
against NRC or the creators of the lexicon, either on your own account or on behalf of any
third party, arising directly or indirectly out of your use of the lexicon. In no event
will NRC or the creators be liable on any theory of liability, whether in an action of
contract or strict liability (including negligence or otherwise), for any losses or
damages incurred by you, whether direct, indirect, incidental, special, exemplary or
consequential, including lost or anticipated profits, savings, interruption to business,
loss of business opportunities, loss of business information, the cost of recovering such
lost information, the cost of substitute intellectual property or any other pecuniary loss
arising from the use of, or the inability to use, the lexicon regardless of whether you
have advised NRC or NRC has advised you of the possibility of such damages. 


We will be happy to hear from you. For example,:
- telling us what you are using the lexicon for
- providing feedback regarding the lexicon;
- if you are interested in having us analyze your data for sentiment, emotion, and other affectual information;
- if you are interested in a collaborative research project. We regularly collaborate with graduate students,
post-docs, faculty, and research professional from Computer Science, Psychology, Digital Humanities,
Linguistics, Social Science, etc.

Email: Dr. Saif M. Mohammad (saif.mohammad@nrc-cnrc.gc.ca, uvgotsaif@gmail.com)


X. ETHICAL CONSIDERATIONS
-------------------------

Please see the papers below (included with the download) for ethical considerations
involved in automatic emotion detection and the use of emotion lexicons. (These also act
as the Ethics and Data Statements for the lexicon.)

- WorryWords: Norms of Anxiety Association for over 44k English Words. Saif M. Mohammad. In
Proceedings of the Empirical Methods on Natural Language Processing (EMNLP 2024, Main),
November 2024, Miami, FL.

- Ethics Sheet for Automatic Emotion Recognition and Sentiment Analysis.
Saif M. Mohammad. Computational Linguistics. 48 (2): 239–278. June 2022.

- Best Practices in the Creation and Use of Emotion Lexicons. Saif M. Mohammad. 
Findings of the Association for Computational Linguistics: EACL 2023. 2023.

Note that the labels for words are *associations* (and not denotations). As noted in the
paper above, they are limited by when the dataset was annotated, by the people that
annotated them, historical perceptions, and biases. (See bullets c through h in the
paper). It is especially worth noting that identity terms, such as those referring to
groups of people may be particularly prone to inappropriate biases. Further, marginalized
groups have historically faced more negative perceptions. 
