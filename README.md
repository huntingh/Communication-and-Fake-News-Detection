# ECE570-Project

## Running the Experiments
### Github
 1. Download "test.tsv", "train.tsv", and "valid.tsv"
 2. Open one of the experiment files. The naming convention is "project_{# number of words}.ipynb". Images 1 and 2 are from "project_10.ipynb"
 3. Click the "Open in colab" button
 ### Colab
 4. Under runtime, click run all 
 5. Under cell one, the "Choose Files" button should appear
 6. Click "Choose Files" and add the three datasets downloaded earlier 
 7. The test should be running and should take anywhere from 10 - 45 minutes to complete. 

## Description
 - Nearly, all code is from Sindhuja Madishetty's experiement found here: https://github.com/SindhuMadi/FakeNewsDetection. 
 - Code I added can be found in the first cell of the jupiter notebook and  the cell with the comment "Below function performs tokenization process as required by bert and roberta models, for a given dataset". Both can be seen below. 
 ![image](https://user-images.githubusercontent.com/54744576/201969117-a4ffe708-4b1c-45c1-addf-3f2c70e1c6d5.png)
 Image 1: Used Colab library to import the data from local files. Reference here: https://towardsdatascience.com/3-ways-to-load-csv-files-into-colab-7c14fcbdcb92 .. 
 
![image](https://user-images.githubusercontent.com/54744576/201968777-671c25fe-02dc-49e1-beb3-d257d043d653.png)
Image 2: This is where I added different versions. 
For each version I 
 - Changed the max_length variable at the top of the cell. 
 - Copy and pasted a section of the version code. 
	 - In image 2, the start of version 0 is visible. Version 0 was the code used in the original experiment. 
	 - Increased the new version identifier to an unused number.
	 - Changed the word length in the function to match the new max_length value. 
 - Changed the version variable to match the new version identifier.  
	 - The second edited cell was 
 ## Dataset
 - I used the same datasets used in the original experiement found here: https://github.com/SindhuMadi/FakeNewsDetection where they downloaded it from Kaggle here: https://www.kaggle.com/datasets/khandalaryan/liar-preprocessed-dataset. 
 - LIAR dataset was created by Willian Yang Wang in this paper "Liar, Liar Pants on fire": A New Benchmark Dataset for Fake News Detection. found here:  https://arxiv.org/abs/1705.00648. 
 - It has 12.8k short statements labeled with “Labeled for truthfulness, subject, context/venue, speaker, state, party, and prior history” sourced from real examples in the original context, “such as political debate. TV ads, Facebook Posts, tweets, inter‐ view(s), news release(s),” and more. 
 - There are six different labels of truthfulness: roughly 1k statements labeled “pants-fire”, and 2.3k statements labeled for each of the rest: “false”, “barely-true”, “half-true”, “mostly-true”, and “true”. 
 - There is also meta-data available for the statements including “party affiliations, current job, home state, and credit history”.
