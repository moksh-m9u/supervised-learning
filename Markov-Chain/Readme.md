# Markov Chain Text Generator (Bigram Model)

This notebook demonstrates a simple **Markov Chain–based text generator** using **bigrams** (pairs of consecutive words).  
It creates a **transition probability matrix** from an input text and then generates new text by randomly selecting the next word based on these probabilities.

## How It Works
1. **Text Cleaning**  
   - Removes punctuation and converts text to lowercase for consistency using Python’s `re` library.

2. **Bigram Generation**  
   - Uses `nltk.ngrams` to create pairs of consecutive words from the cleaned text.

3. **Transition Matrix**  
   - Builds a matrix where each row represents a current word and each column represents a possible next word.  
   - Each cell stores the probability of transitioning from one word to another.

4. **Text Generation**  
   - Starts from a user-provided initial word.  
   - Repeatedly selects the next word using the transition probabilities until the desired length of text is produced.

This simple notebook shows the basic concept of Markov chains applied to natural language processing without relying on heavy machine learning models.
