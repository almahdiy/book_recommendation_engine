# Book Recommendation Engine


### Question/need:
###### What is the framing question of your analysis, or the purpose of the model/system you plan to build?
One of my favorite things to do at my spare time is to read books. In this project, I will build a book recommendation engine based [Goodreads.com] book data. I have previously implemented a recommendation system, but it was basic; it used collaborative filtering (looking at users who have liked similar items and recommend their other likes to the target user) and SVD matrix factorization. For this project, I want to implement content-based filtering, and use unsupervised machine learning and natural language processing to add an additional layer of complexity, by considering the descriptions of the books.
###### Who benefits from exploring this question or building this model/system?
The system will help users find books similar to those they have already read and liked. This is also a proof-of-concept, but the same approach can be used to build recommendation engines for movies, music, online courses, travel destinations, foods, etc, as long as data sets can be found/collected. 

### Data Description:
###### What dataset(s) do you plan to use, and how will you obtain the data?
I found a Goodreads dataset on Kaggle, but it does not contain book descriptions. Therefore, I will attempt to generate my own dataset by web scrapping. 
###### What is an individual sample/unit of analysis in this project? What characteristics/features do you expect to work with?
Book title, description, author, publisher, year of publishing, genre(s), and number of pages. I do not think I should consider star ratings, because it is not a characteristic of the book and people could have different tastes in books, but I might experiment with it. 
###### If modeling, what will you predict as your target?
I will build an unsupervised model, which I can give books that I like and it will tell me which other books are similar to it, based on the similarity/distance/whether they fall in the same cluster as books I have previously liked.

### Tools:
###### How do you intend to meet the tools requirement of the project?
I will most likely use scikit-learn to build my unsupervised model, in addition to text preprocessing and vectorization. 
###### Are you planning in advance to need or use additional tools beyond those required?
Like I said, I will collect data myself, so I will need to use web scrapping libraries such as BeautifuISoap. In addition to Bokeh to generate the report. I know BERT is the cutting-edge NLP technology, but I don’t know much about it and I don’t know if it’s applicable here. I will play around with it as I build my recommender and figure that out.

### MVP Goal:
###### What would a minimum viable product (MVP) look like for this project?
I am thinking an interactive HTML report where user can hover over dots (representing books) in the chart, and see their information, and the other books in the same cluster. 


[Goodreads.com]: https://www.goodreads.com