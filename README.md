## The Corpus and the Intended Use
The corpus consists of the lyrics of 14 songs in Adele's album *25* which was released on November 20, 2015. The corpus can be used by anyone who is interested in Adele's music or this album. 
## Text Selection Criteria
All songs in this album were collected.
## The Data Collection Process
First, I entered the website (https://genius.com/albums/Adele/25). Then, I used BeautifulSoup in Python for web scraping. I extracted the titles and the links of these songs, but the HTML text of lyrics was too complex to understand. Therefore, I had to manually copy the lyrics and pasted them to 14 text files. Furthermore, I wrote a metadata for the data, which recorded the track and the producer of each song.
## Cleaning and Preprocessing Steps
Title(Filename): I called startswith() function to filter out needless information which did not start with "\n".<br/>
Lyric(Document): I removed the extra spaces with replace() function. 
## Annotations and Tools
Annotations: tokenization, lemmatization, part of speech and named entity recognition.<br/>
Tools: BeautifulSoup, pandas and spaCy.
## Files Format and The Description of the Columns
Format: csv & txt <br/>
Description:

## The Quality Checks
In named entity recognition section, I tested the result of the third song called *I Miss You*. Some named entities were inaccurate. For example, "Down" was identified as a person since it's capitalized as the first word in a sentence. Also, "Towards" was recognized as a product. In a word, before we use NER to analyze a text, we need to go through the result first and modify the mistakes. The outcomes based on NER may not be quite reliable. 
