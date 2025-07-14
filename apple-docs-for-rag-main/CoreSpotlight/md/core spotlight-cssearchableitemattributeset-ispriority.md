

- Core Spotlight
- CSSearchableItemAttributeSet
-  isPriority 

Instance Property

# isPriority

A Boolean value that indicates whether the mail or messages content represents a prioritized item.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
var isPriority: NSNumber? { get }
```

## Discussion

When the value of this property is `1`, Apple Intelligence identified this email or message content as needing priority classification.

## See Also

### Describing Apple Intelligence prioritization and summarization

var textContentSummary: String?

A string that presents the Apple Intelligence summarization of the item.

var transcribedTextContent: String?

A string that represents the text the system transcribed.

