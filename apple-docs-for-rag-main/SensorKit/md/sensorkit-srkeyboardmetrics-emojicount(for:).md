

- SensorKit
- SRKeyboardMetrics
-  emojiCount(for:) 

Instance Method

# emojiCount(for:)

Provides the number of typed emojis for the specified sentiment in the report.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
func emojiCount(for category: SRKeyboardMetrics.SentimentCategory) -> Int
```

## Parameters 

`category`  

An estimation of the user’s demeanor.

## Return Value

The total number of typed emojis for a sentiment.

## See Also

### Inferring Sentiment

func wordCount(for: SRKeyboardMetrics.SentimentCategory) -> Int

Provides the number of typed words for the specified sentiment in the report.

enum SentimentCategory

Moods that the framework determines by analyzing the user’s input.

