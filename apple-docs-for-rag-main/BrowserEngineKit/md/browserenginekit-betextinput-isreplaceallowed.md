

- BrowserEngineKit
- BETextInput
-  isReplaceAllowed 

Instance Property

# isReplaceAllowed

Returns whether replacement should be allowed for an editable element.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
var isReplaceAllowed: Bool { get }
```

**Required**

## Discussion

For example, replacement shouldn’t be allowed in password fields or when the selected text is only consists of whitespace.

## See Also

### Replacing text

func replaceSelectedText(String, withText: String)

Replaces the specified `text` with `replacementText`

**Required**

