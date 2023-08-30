# Pandas 🐼 and Git 🫴🏼 task
This task is fully customizable, you can choose to do it however may you like, but you have to do it. You are encouraged to use the internet to search for answers, use information from the task Menna sent you, and use info from this task there. And of course ask your colleagues for help whenever you need it! 🤗
## Pandas 🐼

### 1. What is Pandas?

Pandas is a Python library used for working with data sets, you should know this by now. It has functions for analyzing, cleaning, exploring, and manipulating data. The name "Pandas" has a reference to both "Panel Data", and "Python Data Analysis" and was created by Wes McKinney in 2008.

Speaking of *analyzing, cleaning, exploring, and manipulating* data, what functions can you use for each of these tasks? 🤔:
- **A**nalyze data?
- **C**lean data?
- **E**xplore data?
- **M**anipulate data?

**Fill the table below:**
  

function | what it does | category
------------ | ----------- | ---------
`astype()` | `is used to cast a pandas object to a specified data type` | `Analyze data`
`groupby()` | `is used for grouping the data according to the categories and applying a function to the categories` | `Analyze data`
`sort_values()` | `method to sort a DataFrame by the specified label` | `Analyze data` 
`pivot_table()` | `method is used to create a spreadsheet-style pivot table as a DataFrame.`  | `Explore data` 
`merge()` | `is used to merge DataFrame or named Series objects with a database-style join.`  |  `Analyze data`
`plot()` | ` is used to create a variety of charts from DataFrame objects.`  |  `Explore data`
`corr()` | `is used to compute pairwise correlation of columns, excluding NA/null values.`  | `Manipulate data` 
`cov()` | ` is used to compute pairwise covariance of columns, excluding NA/null values.`  |  `Explore data`
`apply()` | `is used to apply a function along an axis of the DataFrame.`  |  `Manipulate data`
`loc()` | `used to select rows and columns from a DataFrame which uses labels to select rows and columns.`  |  `Explore data`
`iloc()` | `used to select rows and columns from a DataFrame which  uses integer positions.`  |  `Explore data`
`iterrows()` | `is used to iterate over the rows of a DataFrame as (index, Series) pairs.`  |  `Explore data`
`aggregate()` | `is used to apply one or more functions to the columns of a DataFrame.`  | `Manipulate data`

$\rightarrow$ You may insert code snippets here if you like!

### 2. Pandas and NumPy 🔢 [BONUS 🎁](https://www.imdb.com/title/tt1068680/)

Pandas is built on top of the NumPy package, which means that many of the methods in NumPy are also available in Pandas. Data in pandas is often used to feed statistical analysis in SciPy, plotting functions from Matplotlib, and machine learning algorithms in Scikit-learn.

Speaking of NumPy, here are questions about it:

- What is the output of the following code? And why is it so?

``` python
a = np.array([1, 2, 3])
b = np.array([4, 5, 6])
c = np.vstack((a, b))

print(c[1][2])
```
```
output: 6
why: because of [1] is second row, and [2] is third column where zero index.
```


- What is the output of the following code? And why is it so?

``` python
a = np.array([1, 2, 3])
b = np.array([4, 5, 6])
c = np.intersect1d(a, b)

print(c)
```
```
output: []
why: because intersect1d function returns the sorted, unique values that are in both of the input arrays, and there are no common numberes.
```

  
- What is the output of the following code? And why is it so?

``` python
a = np.array([1, 2, 3])
b = np.array([4, 5, 6])
c = np.setdiff1d(a, b)

print(c)
```
```
output: [1 2 3]
why: because setdiff1d function returns the sorted, unique values that are in the first input array but not in the second input array.
```

- Which of the following is a function in NumPy used for carrying out Einstein summations?

    - [ ]  `np.tensordot()`
    - [ ]  `np.dot()`
    - [x]  `np.einsum()`
    - [ ]  `np.outer()`

- The `np.outer` function is primarily intended for:

    - [ ]  Computing the tensor dot product of two arrays.
    - [X]  Computing the outer product of two arrays.
    - [ ]  Computing the inner product of two arrays.
    - [ ]  Computing the cross product of two arrays.


### 3. Pandas and Matplotlib 📈
Pandas can be used to visualize data using a wrapper for `matplotlib.pyplot.plot()`. You can plot data directly from your DataFrame using certain functions.

- What functions can you use to plot data directly from your DataFrame? 🤔
  ```
  there are several function that allow to plot directory from data frame such as:
  
    1. DataFrame.plot(): This function is a wrapper around matplotlib.pyplot.plot() and allows you to create various types of plots, such as line plots, bar            plots, scatter plots, etc.
    2. DataFrame.plot.line(): This function is used for creating line plots from a DataFrame.
    3. DataFrame.plot.bar(): This function is used for creating bar plots from a DataFrame.
    4. DataFrame.plot.scatter(): This function is used for creating scatter plots from a DataFrame.
  ```

- What is the output of the following code? And why is it so?
  ```
  -The code you provided creates a Pandas DataFrame df with dimensions 10x4, filled with random numbers generated from a standard normal distribution using 
   np.random.randn(). The DataFrame has column names 'a', 'b', 'c', and 'd'.

  -Then, it plots a scatter plot using df.plot.scatter() with the 'a' column values as the x-axis and the 'b' column values as the y-axis.
  ```

``` python
df = pd.DataFrame(np.random.randn(10, 4), columns=['a', 'b', 'c', 'd'])
df.plot.scatter(x='a', y='b')
```
- What do you know about `np.random.randn()`? And how does it depend on `np.random.seed()`?
  ```
  -`np.random.randn()`: is a NumPy function that generates an array of random numbers from a standard normal distribution (mean 0, standard deviation 1).
  -`np.random.seed()`: is used to set the seed value for the random number generator in NumPy. you can ensure that the random numbers generated by NumPy are     
    reproducible, meaning that executing the same code with the same seed will produce the same random numbers.
  ```

## Git 🫴🏼
I know you are all familiar with Git, but let's see how much you know about it! 🤓

- What is the default text editor for the Bash shell with a Windows-based Git install?

    - [ ] Emacs
    - [x] Vim
    - [ ] Notepad++
    - [ ] Bash

- Before you install Git, which of the following prerequisite products must be present and configured on your local OS?

    - [ ] Python
    - [ ] Java Development Kit 1.8 or newer
    - [ ] Apache Maven
    - [x] Nothing


- After you install Git and prior to issuing the first commit, which two configuration properties does the tool expect to be configured?

    - [x] username and email address
    - [ ] username and password
    - [ ] email address and password
    - [ ] username and IP address

- Which of the following commands is used to create a new Git repository?

    - [x] git init
    - [ ] git clone
    - [ ] git commit
    - [ ] git push

- Which of the following commands is used to clone a remote Git repository?

    - [ ] git init
    - [x] git clone
    - [ ] git commit
    - [ ] git push

- Which of the following commands is used to stage a file for inclusion in the next commit?

    - [x] git add
    - [ ] git commit
    - [ ] git push
    - [ ] git pull

- Which of the following commands is used to commit staged changes to the local repository?

    - [ ] git add
    - [x] git commit
    - [ ] git push
    - [ ] git pull

- Which of the following commands is used to push committed changes to a remote repository?

    - [ ] git add
    - [ ] git commit
    - [x] git push
    - [ ] git pull

- Who is attributed with inventing Git?

    - [ ] Junio Hamano
    - [ ] James Gosling
    - [ ] Kohsuke Kawaguchi
    - [x] Linus Torvalds

- After you initialize a new Git repository and create a file named git-quiz.html, which of the following commands will not work if issued?

    - [ ] git add git-quiz.html
    - [ ] git status
    - [ ] git add .
    - [x] git commit -m "git quiz web file added"

- Which file can you configure to ensure that certain file types are never committed to the local Git repository?

    - [ ] ignore.git
    - [x] .gitignore
    - [ ] gitignore.txt
    - [ ] git.ignore

- Under which circumstance should you use a single dash within a bash command, as opposed to a double dash?
  ```
  a single dash is used for single-character options and a double dash is used for multi-character options. For example, if you want to list the contents of a 
  directory in long format with human-readable sizes, you can use the command ls -lh. Here -l is a single-character option that stands for long format and -h is 
  another single-character option that stands for human-readable sizes. If you want to use the --help option of the ls command, you would use ls --help.
  ```

- Which vendor acquired GitHub for $7.5 billion in June 2018?
```
'Microsoft'
```

You may want to check [this](https://www.youtube.com/watch?v=Q6G-J54vgKc&t=16813s)

## Problem Solving 🤔
[A. Panoramix's Prediction](https://codeforces.com/problemset/problem/80/A)
```
  n, m = map(int, input().split())
  prime_nums = [2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47]
  
  x = prime_nums.index(n)
   
  if x < 14 and m == prime_nums[x+1]:
      print("YES")
  else:
      print("NO")
```


[A. Again Twenty Five!](https://codeforces.com/problemset/problem/630/A)
```
  n = int(input())
  print(25)
```
