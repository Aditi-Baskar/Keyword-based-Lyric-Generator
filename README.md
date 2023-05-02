# 685: Advanced Natural Language Processing
# Project: Keyword-based Song Lyric Generation

## Contributors
- Aditi Baskar
- Suraj Jain
- Akshaya Mohan
- Niel Parekh

## File Log

### Data files
1. `lyrix.txt`: All TS lyrics in a text file
2. `prompts for keyword extraction.txt`: List of prompts to extract keywords from song lyrics using ChatGPT
3. `ts_data.json`: Cleaned datafile with TS song title, lyrics and keywords
4. `Lyrics_TaylorSwift.json`: `lyricsgenius` generated dump of TS discography details
5. `other_data.json`: Cleaned datafile with 300 songs of other artists with song titl and lyrics


### Code files
1. `prjapi.ipynb`: Code to scrape TS lyrics from Genius website
2. `lg_TS.ipynb`: Code to use `lyricsgenius` library to extract and clean all lyrics by Taylor Swift. JSON file with title and lyrics generated.
3. `lg_other.ipynb`: Code to use `lyricsgenius` library to extract and clean 300 songs of 6 other artists. JSON file with title and lyrics generated.
