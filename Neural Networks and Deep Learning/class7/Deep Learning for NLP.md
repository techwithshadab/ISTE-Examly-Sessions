# Deep Learning for NLP

### Agenda

1. Word Embeddings

2. RNN

3. LSTM

4. Path Ahead



### Word Embeddings

**One-hot encoding**

How are you

This is you



Unique words :- How, are, you, this, is

How :- [1, 0, 0, 0, 0]

are :- [0, 1, 0, 0, 0]

.

.

is :- [0, 0, 0, 0, 1]



These are also sparse vectors



50000 words in vocabulary -> 50000 sized vector



### Word2vec

![](https://miro.medium.com/max/1806/1*cuOmGT7NevP9oJFJfVpRKA.png)

Two ways to solve the same problem

Input is one-hot encoded vector

The output of hidden layer is used as word-embedding



**Word2vec properties**

1. Can find similarities between words

2. woman+king-man closer to queen





## RNN

Repeat A to Z

Now try Z to A

Now start somewhere from middle

Human brain has the sequential memory nature by default

![](https://miro.medium.com/max/1254/1*go8PHsPNbbV6qRiwpUQ5BQ.png)

![](https://pythonmachinelearning.pro/wp-content/uploads/2017/10/Unrolled-RNN.png.webp)

![](https://miro.medium.com/max/269/1*U_-WbACJ-4ng9jImoplJXQ.png)

![](https://miro.medium.com/max/714/0*04-4nua4q2PRqLag.png)

![](https://miro.medium.com/max/218/0*q3pOhx4Esh0zl3cX.png)



### Backpropagation through time

![](https://ars.els-cdn.com/content/image/1-s2.0-S0959438818302009-gr1.jpg)

### Vanishing gradient problem

As the network size becomes bigger the gradient to initial layers might get smaller and thus leading to no training 

Thus RNN are tough to train

Caused due to the tanh function which restricts values to between -1 to 1



This leads to RNN not having capability of capturing long-term dependencies



### LSTM to the rescue

![](https://cdn.analyticsvidhya.com/wp-content/uploads/2017/12/10131302/13-850x326.png)





![](https://colah.github.io/posts/2015-08-Understanding-LSTMs/img/LSTM3-C-line.png)



### Knowledge resources

https://www.reddit.com/r/learnmachinelearning/

https://www.reddit.com/r/MachineLearning/

https://www.reddit.com/r/LanguageTechnology/

https://www.reddit.com/r/computervision/



1. Write blogs, post content on Linkedin
2. Make real-world projects end-to-end
3. Volunteer for open-source or any other project
4. Do continuous learning