# Programming Assignment 1 | Raymundo, Lorenz Nelson L.
#### This is my submission for PA1 (Experiment 1 | Introduction to Python Programming)
This repository contains a Jupyter Notebook (`RAYMUNDO PA1 2ECE-A.ipynb`) that demonstrates three programming exercises using user-defined functions and slicing
#### Part 1: Alphabetize!
The first part of this programming assignment(PA) aims to create a function that takes a string and returns it with its letters in alphabetical order. 
To do this, I created a user-defined function named "alphabet_soup" that takes a string value x. This string shall then be converted into a list of characters using the list I named "m". 
To sort the characters in alphabetical order, I used m.sort, which will sort the characters inside m. The sorted characters will then be stored in an empty string function.
In order to display each character, a for loop was used. What this does is loop through each iteration/character.
I have then assigned a value to the empty string function so that it gets filled with character values.
Finally, I assign a word to string x. It can be any word that you want. The output would display the same word but in alphabetical order.

#### Here is a code for you to try out:

```Python
def alphabet_soup(x): #takes a parameter x (string)

    m = list(x) #converts input string to a list of characters
    m.sort() #sorts characters alphabetically
    sorted_string = "" #empty string to store results

    for z in m: #loops through each iteration/character
        sorted_string = sorted_string + z #empty string + current letter z
    return sorted_string #returns the final sorted string

print(alphabet_soup('hello')) #string "hello" will take the place of x
print(alphabet_soup('hacker')) #string "hacker" will take the place of x
```


#### Part 2: Emoticons!
The second part of this PA aims to create a function that replaces the words "smile", "grin", "sad", and "mad" with their corresponding emoticons.
To do this, I created a user-defined function named "emoticon" which will take a string value x. 
To replace the given words with their corresponding emoticons, I assigned the value for string x to be x.replace("word", "emoticon"). What this does is that when it detects any one of the given words inside a phrase or sentence, it will replace those words with their respective emoticons.
Finally, we assigned either a word, phrase, or sentence to string x. If, for example, you input "You make me smile", the output will be "You make me :)"

#### Here is a code for you to try out:

```Python
def emoticon(x): #takes a parameter x (string)
    
    x = x.replace('smile' , ':)') #if the code detects a string "smile", it will replace it with :)
    x = x.replace('grin' , ':D') #if the code detects a string "grin", it will replace it with :D
    x = x.replace('sad' , ':((') #if the code detects a string "sad", it will replace it with :((
x = x.replace('mad' , '>:(') #if the code detects a string "mad", it will replace it with >:(

    return x #displays x

print(emoticon('You make me smile')) #string "You make me smile" will take the place of x
print(emoticon('I am mad')) #string "I am mad" will take the place of x
print(emoticon('I am so sad')) #string "I am so sad" will take the place of x
print(emoticon('You make me grin')) #string "You make me grin" will take the place of x
```

#### Part 3: Higher Class, Middle Class, Lower Class (Numbers edition)!
The last part of this PA aims to unpack a certain list into three variables: first, middle, and last. To explain this in a manner that is easily understandable, imagine a list that contains the letters a, b, c, and d. The goal of our code is to create an output that looks like this:
first: a
middle: b, c
last: d
Only this time, we will be using the numbers 1 to 6.
The first thing that you have to do is to create a list x that will hold the numbers 1, 2, 3, 4, 5, 6.
The next thing I did was assign a value to first, middle, and last. For 'first', I assigned the index 0 (first number) value of x. For 'middle, I used slicing to get the middle values, x[1:-1], which starts at index 1 and ends just before index -1 (second number to BEFORE the last number). And lastly, for 'last', I assigned the index -1 (last number) value of x. 
The output should look like this:
first: 1
middle: 2,3,4,5
last: 6

#### Here is a code for you to try out:
```Python
x = [1, 2, 3, 4, 5, 6] #creates a list x that holds the numbers 1,2,3,4,5,6

first = x[0] #get the first element using index 0
middle = x[1:-1] #get the middle elements using slicing 
last = x[-1] #get the last element using index -1

#print the variables to show the result
print("first:", first)
print("middle:", middle)
print("last:", last)
```

#### Pre-requisites
- Python 3.0 or later

#### Installation
These codes were created on Jupyter Notebook. Make sure to install Anaconda Navigator and access Jupyter Notebook. It's all for free! Alternatively, you could use VS Code to run the code.

#### How to Run
1.  Download the `RAYMUNDO PA1 2ECE-A.ipynb` file.
2.  Start the Jupyter Notebook server:
3.  Your web browser will open, upload `RAYMUNDO PA1 2ECE-A.ipynb`, and then click on `RAYMUNDO PA1 2ECE-A.ipynb` to open and run the notebook.


