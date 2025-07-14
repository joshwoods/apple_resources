

- BrowserEngineKit
- BETextSelectionDirectionNavigation
-  move(in:by:) 

Instance Method

# move(in:by:)

Moves the cursor in the specified directions by granularity, in response to different key combinations:

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
func move(
    in direction: UITextStorageDirection,
    by granularity: UITextGranularity
)
```

**Required**

## Discussion

Option + left/right = word Option + up/down = paragraph Command + left/right = line Command + up/down = document

