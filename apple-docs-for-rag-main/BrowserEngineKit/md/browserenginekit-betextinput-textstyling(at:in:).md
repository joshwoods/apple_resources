

- BrowserEngineKit
- BETextInput
-  textStyling(at:in:) 

Instance Method

# textStyling(at:in:)

Returns a dictionary containing NSAttributedString keys represeting appearance customizations.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
func textStyling(
    at position: UITextPosition,
    in direction: UITextStorageDirection
) -> [NSAttributedString.Key : Any]?
```

**Required**

## Discussion

For example, text styling information influence the appearance of a correction rect.

## See Also

### Input traits

var extendedTextInputTraits: (any BEExtendedTextInputTraits)?

Object from which the BEExtendedTextInputTraits will be gathered.

**Required**

