## Fake Review Detection using N-grams

Welcome to the Fake Review Detection project! This project is designed to identify and classify fake or fraudulent reviews from genuine ones using the power of N-grams, a text analysis technique. Fake reviews can be a significant problem in online platforms, and this project aims to contribute to my effort of maintaining trust and integrity in online reviews.

**Advantages:** My approach offers several advantages:

   - **Robust Fake Review Detection:** The use of N-grams allows my model to capture subtle linguistic cues often found in fake reviews, making it robust against sophisticated fraudulent attempts.
   
   - **Interpretability:** My model's predictions are interpretable, as we can trace them back to the presence of specific N-grams in the text.

   - **Real-world Applicability:** Fake review detection has practical applications in various industries, including e-commerce, hospitality, and product reviews, where maintaining the integrity of user-generated content is essential.

### Who Can Benefit?

- **E-commerce Platforms:** Online marketplaces can use my model to automatically filter out fake reviews, improving the trustworthiness of their product ratings.

- **Consumers:** Shoppers and consumers can make more informed decisions by relying on trustworthy reviews and avoiding misleading or fake ones.

- **Review Platforms:** Companies that host user reviews can enhance their platforms' credibility by implementing robust fake review detection.

- **Researchers:** N-grams and text analysis enthusiasts can learn from my project's approach to feature engineering and classification.

This project empowers stakeholders to maintain the authenticity of online reviews, providing a more reliable and trustworthy environment for both businesses and consumers.

I hope you find this project insightful and valuable for your endeavors. Please feel free to explore my code, datasets, and results to get a deeper understanding of my approach.

---
# **N-grams**

N-grams are contiguous sequences of n items from a given sample of text or speech. These items can be characters, words, or other units depending on the application. N-grams are commonly used in natural language processing (NLP) and computational linguistics for various text analysis tasks. The "N" in N-grams represents the number of items in each sequence.

Here are some common types of N-grams:

1. **Unigrams (1-grams):** In the context of text, unigrams are single words. For example, in the sentence "I love programming," the unigrams are "I," "love," and "programming."

2. **Bigrams (2-grams):** Bigrams consist of pairs of adjacent words or characters. In the same sentence, the bigrams are "I love" and "love programming."

3. **Trigrams (3-grams):** Trigrams are sequences of three consecutive words or characters. For the sentence, "I love programming," the trigrams are "I love programming."

4. **4-grams, 5-grams, and so on:** These N-grams consist of sequences of four, five, or more adjacent words or characters, depending on the value of "N."

N-grams capture local patterns and dependencies in text data, making them valuable for a wide range of NLP and text analysis tasks. The choice of "N" (the number of items in the sequence) depends on the specific task and the level of context you want to capture.

### **In My Words: N-grams for Capturing Word Order**

In language, sentence meaning depends on the order of words. For instance:

- "*AF watched the movie and slept on the bed.*"

Changing the word order alters the meaning:

- "*AF slept the movie and watched on the bed.*"

N-grams extend the Bag of Words (BoW) technique, enabling the capture of word order. BoW disregards word order, but with N-grams, we can model word sequences, making it useful for various applications.

**BoW:** BoW is a special case of N-grams with N equal to 1, capturing individual word tokens. In contrast, N-grams capture word pairs, like a moving window.

- **Bigram Example:** "AF-watched," "watched-the," "the-movie," etc.

- **Trigram Example:** "AF-watched-the," "watched-the-movie," "the-movie-and," etc.

The generic term for this concept is 'n-gram,' which can be 4-gram, 5-gram, and beyond. N-grams reveal meaningful word sequences.

## **Limitations of Bag of N-grams Model:**

1. As "n" increases, dimensionality and sparsity increase.

2. The model doesn't address the out-of-vocabulary (OOV) problem.
