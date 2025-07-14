

- Natural Language
-  Finding similarities between pieces of text 

Article

# Finding similarities between pieces of text

Calculate the semantic distance between words or sentences.

## Overview

Finding semantic similarities between words or sentences can help you create a better user experience for your app. For example, you might enhance the experience of searching for specific photos by knowing that the search term “cloud” is related to the word “sky,” and expanding the search query to return more relevant results.

To find similarities between pieces of natural language text, you use text embeddings. An *embedding* is a map from strings—words or sentences—into a vector space. Strings that are semantically similar have similar vectors, which means they’re closer together in vector space.

You use embeddings for tasks like:

- Searching for the nearest neighbors to a given term—for example, to expand a search query.

- Calculating the distance between terms, as a measure of semantic similarity.

- Using the vectors as an input layer for a model.

In Natural Language, NLEmbedding represents an embedding, stored in a space- and time-efficient format. NLEmbedding provides pretrained word embeddings for a number of languages, trained on large bodies of general text.

### Find similar words

To calculate the distance between individual words, use a word embedding.

1.  Create an instance of NLEmbedding with wordEmbedding(for:), specifying the language for which to generate a word embedding.

2.  Call the vector(for:) method of the embedding with a specific input word to see the vector generated for that word.

3.  To find the distance between your input word and another word, use `distance(between:and:distanceType:)`.

4.  To find the nearest neighbors to your input word, enumerate over the word’s neighbors by calling the enumerateNeighborsForString:maximumCount:distanceType:usingBlock: method, specifying the maximum number of nearest neighbors to look at.

```
if let embedding = NLEmbedding.wordEmbedding(for: .english) {
    let word = "bicycle"

    if let vector = embedding.vector(for: word) {
        print(vector)
    }

    let specificDistance = embedding.distance(between: word, and: "motorcycle")
    print(specificDistance.description)

    embedding.enumerateNeighbors(for: word, maximumCount: 5) { neighbor, distance in
        print("\(neighbor): \(distance.description)")
        return true
    }
}
```

### Find similar sentences

To calculate the distance between phrases, use a sentence embedding. You might use it to measure similarity between sentences for tasks like text retrieval, or for detecting paraphrases. For example, if a user searches a food-delivery app using the text, “Where is my order?” you could use a sentence embedding to suggest a result from the FAQ with the similar title, “How do I check the status of my order?”

1.  Create an instance of NLEmbedding with sentenceEmbedding(for:), specifying the language for which to generate a sentence embedding.

2.  Call the vector(for:) method of the embedding with a specific input sentence to see the vector generated for that sentence.

3.  To find the distance between your input sentence and another sentence, use distanceBetweenString:andString:distanceType:.

```
if let sentenceEmbedding = NLEmbedding.sentenceEmbedding(for: .english) {
    let sentence = "This is a sentence."

    if let vector = sentenceEmbedding.vector(for: sentence) {
        print(vector)
    }

    let distance = sentenceEmbedding.distance(between: sentence, and: "That is a sentence.")
    print(distance.description)
}
```

Sentence embeddings are dynamic. They don’t have a fixed vocabulary, and they can return results for arbitrary sentences. Nearest-neighbor search therefore doesn’t apply to sentence embeddings.

## See Also

### Text embedding

class NLEmbedding

A map of strings to vectors, which locates neighboring, similar strings.

