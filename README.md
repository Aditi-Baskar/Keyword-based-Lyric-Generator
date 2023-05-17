# 685: Advanced Natural Language Processing
# Project: Keyword-based Song Lyric Generation

## Contributors
- Aditi Baskar
- Akshaya Mohan
- Niel Parekh
- Suraj Jain

## File Log

### Data files
1. `lyrix.txt`: All TS lyrics in a text file
2. `prompts for keyword extraction.txt`: List of prompts to extract keywords from song lyrics using ChatGPT
3. `ts_data.json`: Cleaned datafile with TS song title, lyrics and keywords
4. `Lyrics_TaylorSwift.json`: `lyricsgenius` generated dump of TS discography details
5. `other_data.json`: Cleaned datafile with 300 songs of other artists with song titl and lyrics
6. `song_lyrics.csv`: File with the lyrics and labels of all the songs in the json files
7. `q1.txt`, `q2.txt`: prompt and song for few shot prompting
8. `a1.txt`, `a2.txt`: keywords outputs for few shot prompting
9. `songs_pt1.json`, `songs_pt2.json`: two splits of input dataset for keyword generation
10. `json_songspt1_keywords.json`, `json_songspt2_keywords.json`: two splits of dataset with generated keywords (generated by keyword_generation.ipynb)
11. `final_dataset.json`: cleaned and combined songs dataset with keywords (generated by final_dataset.ipynb)
12. `t5_testing.csv`: original and T5 generated lyrics for test set
13. `t5_testing_keywords.csv`: keywords generated by gpt-3.5-turbo for the T5 generated test set lyrics
14. `semantic_evaluation.csv`: max, min and average cosine similarities for gold and generated keywords for test set
15. `ngram.csv`: lyrcis generated by the n gram model given the first line for the song
16. `ngram_with_key.csv`: lyrcis generated by the n gram model given the keywords for the song



### Code files
1. `prjapi.ipynb`: Code to scrape TS lyrics from Genius website
2. `lg_TS.ipynb`: Code to use `lyricsgenius` library to extract and clean all lyrics by Taylor Swift. JSON file with title and lyrics generated.
3. `lg_other.ipynb`: Code to use `lyricsgenius` library to extract and clean 300 songs of 6 other artists. JSON file with title and lyrics generated.
4. `json_to_csv.ipynb`: Code to convert the data in the json files into csv file to be used by the BERT classifier.
5. `data_split.ipynb`: clean and split the songs dataset
6. `keyword_generation.ipynb`: generate keywords for the songs using gpt-3.5-turbo
7. `final_dataset.ipynb`: clean and combine the split datasets with keywords to form the final training dataset
8. `t5_fine_tuning.ipynb`: fine tune T5 model on keywords and lyrics
9. `semantic_evaluation.ipynb`: compute cosine similarity for the keywords generated from test set lyrics
10. `Ngram.ipynb`: Code to create n gram model(baseline model 1) and generate text
11. `Ngram_with_keyword.ipynb`: Code to create n gram model including keywords(baseline model 2) and generate text
12. `bert_2.ipynb`: Code to train the bert classifier to perform stylistic evaluation 
