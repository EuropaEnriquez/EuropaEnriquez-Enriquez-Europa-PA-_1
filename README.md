**1. Alphabet Soup Problem**
Create a function that takes a string and returns a string with its letters sorted in alphabetical order.

```
def alphabet_soup(word):
    return word[::-1]
print(alphabet_soup("hello")) 
print(alphabet_soup("world"))
```
How the works: 
This function uses built-in sorted() function to sort the letters of the input string alphabetically, then joins the sorted letters back into a single string before returning it.

Example:
```
Input: "hello"
Output: "olleh"
```

**2. Emoticon Problem**
Create a function that converts specific words in a sentence to their matching emoticons. The words replaced are "smile" → ":)", "grin" → ":D", "sad" → ":(", and "mad" → ">:("
```
def emotify(sentence):
    words = sentence.split()
    result = ""
    for word in words:
        if word == "smile":
            result += ":) "
        elif word == "grin":
            result += ":D "
        elif word == "sad":
            result += ":( "
        elif word == "mad":
            result += ">:( "
        else:
            result += word + " "
    return result


print(emotify("Make me smile"))
print(emotify("Make me mad"))
print(emotify("Make me sad"))
print(emotify("Make me grin"))
```
How the code works:  
The function `emotify(sentence)` splits the input sentence into words and iterates over them. When a word matches one of the target words, it inserts the corresponding emoticon into the result string. Other words remain unchanged. It returns the sentence with emoticons replacing the specified words.

```
Example:
Input: "Make me smile"
Output: "Make me :)"
```


**3. Unpacking List Problem**
Given a list, unpack it into three variables: first element, middle elements as a sublist, and last element. Then print these variables.

```
lst = [1, 2, 3, 4, 5, 6]

first = lst[0]
middle = lst[1:-1]
last = lst[-1]

print("first:", first)
print("middle:", middle)
print("last:", last)
```

How the code works:  
A list `lst` is defined. The first element is assigned to `first`, the middle elements (everything except the first and last) to `middle`, and the last element to `last`. These variables are printed showing the unpacked parts of the list.

```
Example:  
Input:[1][2]

Output:  
first: 1  
middle:[2]
last: 6
```

**REVISION #1 (Revised problem 1)**

**PROBLEM 1**

```
def alphabet_soup(word):
    return ''.join(sorted(word))
print(alphabet_soup("hello"))  
print(alphabet_soup("world"))  
```

How the code works:  
This function uses built-in sorted() function to sort the letters of the input string alphabetically, then joins the sorted letters back into a single string before returning it.
```
Example:
Output: ehllo
        dlorw
```


