

- Assignables
- AssignableDocument
-  computeMaxScore(defaultQuestionMaxScore:) 

Instance Method

# computeMaxScore(defaultQuestionMaxScore:)

Computes the maximum possible score for this `AssignableDocument` as defined by each individual question’s `maxScore`.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
func computeMaxScore(defaultQuestionMaxScore: Double? = Double.zero) -> Double?
```

## Parameters 

`defaultQuestionMaxScore`  

If a question has a `nil` `maxScore` value, the value that should be used instead.

## Return Value

The maximum possible score for this `AssignableDocument` as defined by each individual question’s `maxScore`. `nil` is returned, if any individual’s `maxScore` is `nil` and `defaultQuestionMaxScore` is `nil`.

