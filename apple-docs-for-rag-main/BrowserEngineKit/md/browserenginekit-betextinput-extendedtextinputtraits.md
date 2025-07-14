

- BrowserEngineKit
- BETextInput
-  extendedTextInputTraits 

Instance Property

# extendedTextInputTraits

Object from which the BEExtendedTextInputTraits will be gathered.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
var extendedTextInputTraits: (any BEExtendedTextInputTraits)? { get }
```

**Required**

## See Also

### Input traits

func textStyling(at: UITextPosition, in: UITextStorageDirection) -> [NSAttributedString.Key : Any]?

Returns a dictionary containing NSAttributedString keys represeting appearance customizations.

**Required**

