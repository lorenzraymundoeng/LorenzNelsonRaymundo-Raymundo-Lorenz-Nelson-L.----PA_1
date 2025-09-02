# LorenzNelsonRaymundo/Raymundo-Lorenz-Nelson-L.----PA_1
#### This is my submission for PA1 (Experiment 1 | Introduction to Python Programming)
#### Part 1:
The first part of this programming assignment(PA) aims to create a function that takes a string, and returns it with its letters in alphabetical order. 
To do this, I created a user-defined function named "alphabet_soup" which will take a string value x. This string shall then be converted into a list of characters using the list I named as "m". 
To sort the characters in alphabetical order, I used m.sort, which will sort the characters inside m. The sorted characters will then be stored to an empty string function.
In order to display each character, for loop was used. What this does is that it loops through each iteration/character.
I have then assigned a value to the empty string function so that it gets filled with character values.
Finally, I assign a word to string x. It can be as many as you want. The output would display the same word but in alphabetical order.

#### Here is a code for you to try out:

```
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


#### Part 2:
The second part of this PA aims to create a function that replaces the words "smile", "grin", "sad", and "mad" with their corresponding emoticons.
To do this, I created a user-defined function named "emoticon" which will take a string value x. 
To replace the given words with their corresponding emoticons, I assigned the value for string x to be x.replace("word", "emoticon"). What this does is that when it detects any one of the given words inside a phrase or sentence, it will replace those words with their respective emoticons.
Finally, we assigned either a word, phrase, or sentence to string x. If, for example, you input "You make me smile", the output will be "You make me :)"

#### Here is a code for you to try out:

```
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




#### We were instructed to (1) Create a function that takes a string and returns a string with its letters in alphabetical order. (2) Create a function that changes specific words into emoticons. Given a sentence as a string, replace the words smile, grin, sad, and mad with their corresponding emoticons. (3) Unpack the list into three variables, being first, middle, and last, with middle being everything between the first and last element. Then print all three variables.

