

- SensorKit
- SRKeyboardMetrics
-  SRKeyboardMetrics.SentimentCategory 

Enumeration

# SRKeyboardMetrics.SentimentCategory

Moods that the framework determines by analyzing the user’s input.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
enum SentimentCategory
```

## Overview

This class describes possible values for wordCount(for:) and emojiCount(for:) properties of a keyboard report.

## Topics

### Sentiments

case absolutist

A mood that embodies absolutism.

case anger

A mood that embodies anger.

case anxiety

A mood that embodies worrying.

case confused

A mood that embodies confusion.

case death

A mood that expresses death.

case down

A mood that embodies depression.

case health

A general concern for health.

case lowEnergy

A mood that indicates low energy.

case positive

A mood that embodies positivity.

case sad

A mood that embodies sadness.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inferring Sentiment

func wordCount(for: SRKeyboardMetrics.SentimentCategory) -> Int

Provides the number of typed words for the specified sentiment in the report.

func emojiCount(for: SRKeyboardMetrics.SentimentCategory) -> Int

Provides the number of typed emojis for the specified sentiment in the report.

