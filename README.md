# Shakespeare Text Generation using Markov Chains

This project uses Markov Chains to generate Shakespeare-like text. It demonstrates the application of stochastic methods in natural language processing.

## Setup
1. Install required libraries: `pip install markovify matplotlib nltk pandas seaborn`
2. Run the Python Notebook.

## Project Structure
- `HMM_Text_Gen.py`: Main Python Notebook
- `README.md`: Project documentation

## Methodology
1. Preprocess the text
2. Build a Markov Chain model using Markovify
3. Generate new text using the model
4. Analyze and visualize the original and generated text
5. Compare and evaluate the model

## Analysis of Results

### Word Frequency Distribution
The model successfully captures the high-frequency words typical of Shakespeare's writing style. Common words like articles and prepositions appear with similar frequencies in both the original and generated texts. This indicates that the model has learned the basic structure of Shakespearean English.

### Sentence Length Distribution
While the model replicates the general pattern of sentence lengths found in Shakespeare's works, it shows a tendency to produce a wider range of sentence lengths. This could result in some sentences that feel either too short or too long compared to Shakespeare's style. The broader distribution might add variety to the generated text but could occasionally produce sentences that don't quite match the rhythmic patterns of Shakespearean writing.

### Bigram Analysis
The comparison of bigram frequencies between the original and generated texts reveals that the model has captured many of the word-pair patterns present in Shakespeare's writing. However, the scatter plot shows some deviation from a perfect correlation, indicating that the model doesn't replicate these patterns exactly. This balance between mimicry and variation is a key feature of the Markov Chain approach, allowing for text generation that feels Shakespearean without being a direct copy.

### Vocabulary and Sentence Uniqueness
- Vocabulary Overlap (1.87%): The low overlap suggests that the model is generating a wide range of words, including many not present in the training text. This could be seen as a form of creativity, but it also risks producing anachronistic or out-of-style words that wouldn't appear in Shakespeare's works.
- Unique Sentence Ratio (0.22%): This very low ratio indicates that almost all generated sentences are unique combinations rather than copies from the original text. This is a positive sign, showing that the model is creating new content rather than simply reproducing memorized phrases.

### Strengths of the Model
1. Captures basic sentence structure and common word usage patterns.
2. Produces a variety of sentence lengths, adding diversity to the generated text.
3. Creates mostly unique sentences, demonstrating the ability to generate novel content.

### Limitations and Areas for Improvement
1. May occasionally produce anachronistic or out-of-style words not fitting Shakespeare's language.
2. Sentence length variation might sometimes result in structures that feel un-Shakespearean.
3. Limited ability to maintain long-term context or thematic consistency across multiple sentences.

### Potential Applications
1. Creative writing assistance for Shakespeare-inspired works.
2. Educational tools for studying Shakespearean language patterns.
3. Generation of dialogue for Shakespeare-themed games or interactive experiences.

### Future Work
1. Experiment with different state sizes in the Markov Chain to balance between coherence and creativity.
2. Incorporate part-of-speech tagging to improve grammatical accuracy.
3. Implement a more sophisticated language model (e.g., LSTM or Transformer-based) for comparison.
4. Develop a method to maintain thematic consistency across longer generated passages.

This project demonstrates the potential and limitations of using Markov Chain models for text generation in a specific stylistic context. While it captures many surface-level features of Shakespearean writing, it also highlights the complexity of truly replicating the nuanced, context-dependent nature of human-authored text.

## Conclusion
This project demonstrates the application of stochastic methods (Markov Chains) to text generation. While it can produce Shakespeare-like text, it also shows the limitations of this approach in capturing the full complexity of natural language.
