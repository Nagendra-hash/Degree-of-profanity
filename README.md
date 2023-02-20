# Degree-of-profanity
## About
This Python program reads in a file of Twitter tweets, and a set of racial slurs, and calculates the degree of profanity for each sentence in the file. The program assumes that the tweets are stored in a text file, with one tweet per line, and that the set of racial slurs is provided as a Python set, with one slur per element.

## Requirements

* Python 3.x

## Usage

1.Clone the repository to your local machine.   
2.Ensure that you have Python 3.x installed.   
3.Open a terminal and navigate to the root of the cloned repository.   
4.Run the following command: python tweets.py.    
5.The program will read in the file of tweets, calculate the degree of profanity for each tweet, and print the results to the console.

## Customization

You can customize the program by changing the name of the input file, and by adding or removing racial slurs from the set. To change the name of the input file, edit the following line in tweets.py:   

    with open('tweets.txt', 'r') as f:
To add or remove racial slurs, edit the following line in tweets.py:   

    racial_slurs = {'slur1', 'slur2', 'slur3', ...}
