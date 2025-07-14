

- BrowserEngineKit
- BETextSelectionDirectionNavigation
-  extend(in:by:) 

Instance Method

# extend(in:by:)

Moves the selection in the specified directions by granularity, in response to different key combinations:

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
func extend(
    in direction: UITextStorageDirection,
    by granularity: UITextGranularity
)
```

**Required**

## Discussion

Word = shift + option + left/right paragraph = shift + option + up/down line = shift + command + left/right document = shift + command + up/down

