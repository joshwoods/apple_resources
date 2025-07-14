

- Create ML
- MLRecommenderMetrics
-  init(precisionRecall:excludingObserved:) Deprecated

Initializer

# init(precisionRecall:excludingObserved:)

Creates metrics for a recommender, given a data table with precision and recall metric columns, and whether the recommender omitted training data.

macOS 10.15–14.0Deprecated

``` source
init(
    precisionRecall: MLDataTable,
    excludingObserved: Bool
)
```

## Discussion

Do not use this initializer. MLRecommender generates metrics for you when you call its `MLRecommender/evaluation(on:userColumn:itemColumn:ratingColumn:cutoffs:excludingObserved:)` method.

