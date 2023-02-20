# Degree-of-profanity

    def calculate_profanity(tweet, slurs):
        """Calculates the degree of profanity for a single tweet."""
        words = tweet.split()
        num_slurs = len(set(words).intersection(slurs))
        return num_slurs / len(words) if len(words) > 0 else 0

    def main():
        # Set of racial slurs
        racial_slurs = {'slur1', 'slur2', 'slur3'}

        # Open file of tweets and calculate profanity for each tweet
        with open('tweets.txt', 'r') as f:
            for i, line in enumerate(f):
                tweet = line.strip()
                profanity = calculate_profanity(tweet, racial_slurs)
                print(f'Tweet {i+1}: {tweet}\nProfanity: {profanity:.2%}\n')

    if __name__ == '__main__':
        main()



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
 
## Commits and Comments

> Commit 1   
    
    Add tweets.txt file with sample tweets   
   
  This commit adds a file called tweets.txt to the repository, which contains some sample Twitter tweets.
> Commit 2   

    Define racial slurs set in tweets.py
  This commit defines a set of racial slurs in the tweets.py file, which will be used to calculate the degree of profanity for each tweet.
> Commit 3

    Add calculate_profanity function to tweets.py
  This commit adds a calculate_profanity function to the tweets.py file, which takes in a tweet and a set of racial slurs, and calculates the degree of profanity for the tweet.
> Commit 4

    Add main loop to tweets.py
 
This commit adds a main loop to the tweets.py file, which reads in the file of tweets, calculates the degree of profanity for each tweet using the calculate_profanity function, and prints the results to the console.
