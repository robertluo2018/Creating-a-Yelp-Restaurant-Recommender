# Abstract

## About the Author
This project was completed by Robert Luo, an Applied Mathematics student at Northwestern University (graduating Spring 2018). Please feel free to send comments or feedback to robertluo@u.northwestern.edu. An in-depth report of this project can be downloaded in the .zip file linked above. [download][https://robertluo2018.github.io/Yelp-Restaurant-Recommender/project_proposal_RobertLuo.pdf]


## About the Project
Yelp is an online platform where users can submit reviews about restaurants and businesses. A business' Yelp rating and its written reviews can attract or repel visitors, and consequently determine the success of the business. Many consumers depend on Yelp as well. In today's day and age, access to crowd-sourced reviews can highly influence consumer decisions on what stores to shop at and restaurants to dine in. A model that can predict when a Yelp reviewer will rate a restaurant highly (4 or 5 stars) can serve as a valuable recommender system, increasing user engagement and retention as well as customer traffic to new restaurants.

This project evaluates the performance of User-Item Collaborative Filtering, Item-Item Collaborative Filtering, and K-Nearest Neighbor Collaborative Filtering in predicting Yelp user ratings of restaurants in the United States.

#### To define these methods:
- User-Item CF: "Users similar to you liked..."
- Item-Item CF: "Users who liked this restaurant also liked..."
- K-NN CF: "You might like this item based on your ratings of K similar items..."

[I downloaded my dataset from the Yelp dataset challenge,](https://www.yelp.com/dataset/challenge) and used data consisting of user reviews and business features. I created a matrix of user-restaurant-ratings to use with User-Based and Item-Based CF, which I also used for K-NN CF in conjunction with a one-hot matrix of restaurants and their attributes. Due to the size of the  Yelp dataset, I chose to only consider users and restaurants in the US with at least 15 reviews in order to avoid the cold-start problem related to recommender systems (this remains unaddressed throughout the project). Some of the features considered in the one-hot matrix used for K-NN CF include: cuisine type, restaurant attire, ambience, alcohol availability, and price range. Categorical variables were converted to one-hot attributes, for a total of 170 attributes. I used scikit-learn to assist with the project, along with some implementation of my own. Code and processed data can be found in the repository.

## Results
Insert results here (with at least one figure)




# Acknowledgements
The following guides were very helpful for the implementation of my project:
- [Implementing Your Own Recommender Systems in Python](https://cambridgespark.com/content/tutorials/implementing-your-own-recommender-systems-in-Python/index.html)
- [Intro to Recommender Systems: Collaborative Filtering](http://blog.ethanrosenthal.com/2015/11/02/intro-to-collaborative-filtering/)



You can use the [editor on GitHub](https://github.com/robertluo2018/EECS-349-Final-Project/edit/master/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/robertluo2018/EECS-349-Final-Project/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
