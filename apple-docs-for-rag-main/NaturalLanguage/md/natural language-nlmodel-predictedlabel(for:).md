

- Natural Language
- NLModel
-  predictedLabel(for:) 

Instance Method

# predictedLabel(for:)

Predicts a label for the given input string.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func predictedLabel(for string: String) -> String?
```

## Parameters 

`string`  

The input text for the model to analyze.

## Return Value

The model’s predicted label for the input string.

## See Also

### Making predictions

func predictedLabels(forTokens: [String]) -> [String]

Predicts a label for each string in the given array.

func predictedLabelHypotheses(for: String, maximumCount: Int) -> [String : Double]

Predicts multiple possible labels for the given input string.

func predictedLabelHypotheses(forTokens: [String], maximumCount: Int) -> [[String : Double]]

Predicts multiple possible labels for each string in the given array.

