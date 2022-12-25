# Small_projects_in_course_web_analytics
<br>
<h2>Word selection  </h2>
 
 I had to create a pyhon notebook and create 1 method with the name select. Select took 2 parameters , 1 list with strings and L and a dictionary D.
 The dictionary has strings like keys. Every key is correlated with a list with 2 integers. <br>
 <br>
 For example: 
 <br>
L=['table', 'apple', 'orange', 'room', 'person', 'room', 'room', 'person','orange']  <br>
D={'table':[2, 5], 'chair':[0, 2], 'room':[2, 4], 'food':[3, 20]} <br>
<BR>
The method select has to return a list that contains every word w and meets 3 criteria: <br>
* The word w must be included in the given dictionary D and given list L. <br>
* The frequency of word w in list L must be greater than or equal to the first integer in list D[w]. <br>
* The frequency of word w in list L must be less than or equal to the second integer in list D[w].<br>

In the above example : <br>
* The word 'table' does not meet the criteria, since its frequency in L is 1, and 1 < 2 <br>
* The words 'orange', 'apple', 'person', 'food' do not meet the criteria, as they do not appear in both D and L
* The word 'room' meets the criteria, since its frequency in L is 3, and 2<=3<=4

<h2>RottenTomatoes</h2>

* Create a Python Notebook named RottenScraper.ipynb

* Notebook must contain a method named scrape()

* The method must take as a parameter the link for the page with the verified reviews of a movie on rottentomatoes. E.g https://www.rottentomatoes.com/m/the_good_nurse/reviews?type=verified_audience

* The method should create a csv file named reviews.csv.

* The file must contain one line for each of the verified reviews on the first page.

* Each line must contain the name of the reviewer, the rating (in numerical form), and the date of the review. 

For example from this <a href="https://www.rottentomatoes.com/m/the_good_nurse/reviews?type=verified_audience" target="_blank">link</a> we will get a csv file that will write: <br>

John R,5,"Oct 28, 2022"   <br>
Dave,5,"Oct 22, 2022"   <br>
Janice W,4,"Oct 22, 2022"   <br>

<h2>Analyze Movie</h2>

* Create a Homework2.ipynb Notebook (you will find it inside the analyzemovie folder)
* The Notebook must contain an analyze_movie( ) method that takes 3 parameters:
  * input_file: The name of a movie information file. This file will have exactly the same structure as the IMDB-Movie-Data.csv (You can find this csv in the same folder too)
  * actor_name: The name of a specific actor (string). Eg actor_name='Ryan Gosling'
  * stopwords: A set of words (set)
* The method should print a barplot with the 20 most frequent words from the Descriptions of the movies in which the given actor plays. A bar for each of the top 20 words. The height of the bar must be equal to its frequency.
* The method must ignore all words from the stopwords set. These words should not appear in the barplot.

<h2>Trainer (comming) </h2>

* Create a Python Notebook that trains a classifier on the reviews of train_data.csv and uses it to predict the labels for the reviews of test_data.csv.
* The Notebook should print the accuracy of the classifier (one accuracy only, not many accuracies from many different models).
* You can use any classifier you want and tune any parameters you want.
