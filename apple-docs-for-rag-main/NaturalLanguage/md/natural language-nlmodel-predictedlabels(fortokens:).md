

- Natural Language
- NLModel
-  predictedLabels(forTokens:) 

Instance Method

# predictedLabels(forTokens:)

Predicts a label for each string in the given array.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func predictedLabels(forTokens tokens: [String]) -> [String]
```

## Parameters 

`tokens`  

An array of input strings for the model to analyze.

## Return Value

The model’s predicted labels for each of the input strings.

## See Also

### Making predictions

func predictedLabel(for: String) -> String?

Predicts a label for the given input string.

func predictedLabelHypotheses(for: String, maximumCount: Int) -> [String : Double]

Predicts multiple possible labels for the given input string.

func predictedLabelHypotheses(forTokens: [String], maximumCount: Int) -> [[String : Double]]

Predicts multiple possible labels for each string in the given array.

