# Graph approach to Solving the “Six Degrees of Kevin Bacon” problem!

![image info](./pics/KevinBacon6degrees.png)

(Image Credit: https://www.iceinstitute.org/blog/2019/4/1/six-degrees-of-kevin-bacon-education-edition)

## Objective

Create a data generator based on determining the degree of association/relation people have between each other within a given industry. 


## Dataset

Dataset: Netflix Movies and TV Shows
Link: https://www.kaggle.com/shivamb/netflix-shows

## Overview of my First Approach

## Step 1. Convert CSV to Dictionary

![image info](./pics/Step1.png)

## Step 2. Load dictionary to Graph to create distance matrix for actors and directors

![image info](./pics/Step2.png)

## Step 3. Data Generator

![image info](./pics/Step3.png)


Example for Distance Matrix Size of 12:

```
dist_mat = generate_batch_iterator(dictionary, size=12)

next(dist_mat)

```

![image info](./pics/output.png)


## Step 4. Loop through shuffled batches

![image info](./pics/Step4.png)


## Future Directions

- [ ] Improve the efficiency of the batching (using DataLoader)
- [ ] Implement NLP techniques (lower case, spelling check, stemming, lemmatization, vector embedding, etc.)




