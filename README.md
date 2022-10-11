# DBpedia_summarizer


## Data preparation
1. Download DBpedia abstract file (.ttl) in required language [source](http://downloads.dbpedia.org/2015-04/ext/nlp/abstracts/) and put in in the [full_abstracts](/full_abstracts/) folder.
2. Download DBpedia shorteabstract file (.ttl) in required language [source](https://databus.dbpedia.org/dbpedia/text/short-abstracts/) and unzip it in the [short_abstracts](/short_abstracts/) folder.
3. Run the [data_creation notebook](/data_creation.ipynb). Final dataframes should be located in [data](/data/) folder.



## Pretrained models

1. Data for generating summaries located in [data](/data/) folder in .csv files.
2. Notebook [baselines.ipynb](/baselines.ipynb) contains code for running pretrained models (T5, BART and BART-CNN).
3. Generated summaries storing in the dataframe files in separate columns ([example](/data/t5sum_nl_1000.csv), [example](/data/BARTsum_nl_534.csv)).