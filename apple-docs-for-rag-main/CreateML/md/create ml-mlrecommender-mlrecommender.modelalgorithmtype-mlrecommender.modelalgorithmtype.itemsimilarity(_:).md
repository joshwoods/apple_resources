

- Create ML
- MLRecommender
- MLRecommender.ModelAlgorithmType
-  MLRecommender.ModelAlgorithmType.itemSimilarity(\_:) 

Case

# MLRecommender.ModelAlgorithmType.itemSimilarity(\_:)

An algorithm that compares the similarity from item to item.

macOS 10.15+

``` source
case itemSimilarity(MLRecommender.SimilarityType)
```

## Discussion

The default value is MLRecommender.SimilarityType.jaccard.

## See Also

### Recommender algorithms

enum SimilarityType

The metric by which the recommender computes item similarity.

