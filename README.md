# PA3_Programming-Assignment

Author: Noah Oliver H. Nazal  
Date: 09/16/2025  
Course: ECE2112 – Programming Assignment  

# Software(s) Used:
- Anaconda Navigator  
- Jupyter Notebook  

# Repoistory Information
About: Contains solutions for PA 3 (2 Problems)  

# Languages Used
- Pyhton (100%)

# Version History
V1.0 ([09-10-2025]) – Initial Coding for PA1  

V1.1 ([09-15-2025]) - Creation of Repository Along with Read Me file  

V1.2 ([09-16-2025]) – Finalization of Coding PA3 and Edited Documentation, Code Formatting, and Design in the README File  

# Problem 1: Pandas DataFrame Loading
Loads Cars dataset into a Pandas DataFrame named cars and displays the first and last five rows.

Steps: 
Import pandas as pd.
Load the dataset Cars.csv into a DataFrame named cars.
Display the first 5 rows using .head().
Display the last 5 rows using .tail().

# Problem 1: PANDAS DATAFRAME LOADING
# Input
    # Input of word
    x = input("Enter a string:")

    # Sorting word alphabetically
    x_sorted = sorted(x)

    # Output of sorted word
    alpha_sorted = "".join(x_sorted)

    print(alphabet("noah"))

# Output (example)
    ahno
# Problem 2: Subsetting, Slicing, and Indexing
Use the same DataFrame cars from Problem 1 and extracts specific data using subsetting, slicing, and indexing.

# Problem 2: SUBSETTING, SLICING, INDEXING
# Input
    def emoticon(sentence):
        # Make dictionary for word-emoticon equivalents
        replacements = {
            "smile": ":)",
            "grin": ":D",
            "sad": ":((",
            "mad": ">:("
        }

        # Temporary storage of characters
        word = ""
        result = ""

        for ch in sentence:
            if ch != " ":
                word += ch
            else:
                # Process word when space is found
                if word in replacements:
                    result += replacements[word]
                else:
                    result += word
                result += " "
                word = ""

        # After loop, process last word
        if word != "":
            if word in replacements:
                result += replacements[word]
            else:
                result += word

        return result

    # Example:
    x = input("Enter a sentence: ")
    print(emoticon(x))

# Output (example)
    I am :(( but I try to :)

# Problem 3: Unpacking List Problem
Unpack a list into first, middle, and last elements

lst = [1, 2, 3, 4, 5, 6]

# Problem 3: UNPACKING LIST PROBLEM
# Input
    # Starting list
    writeyourcodehere = [1, 2, 3, 4, 5, 6]

    # Breaking into segments
    first, *middle, last = writeyourcodehere

    # Output
    print("first:", first)
    print("middle:", middle)
    print("last:", last)

# Output
    first: 1  
    middle: [2, 3, 4, 5]  
    last: 6  
