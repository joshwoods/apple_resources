

- InputMethodKit
- IMKInputController
-  cancelComposition() 

Instance Method

# cancelComposition()

Stops the current composition and replaces marked text with the original text.

macOS 10.5+

``` source
func cancelComposition()
```

## Discussion

This method calls the method originalString: to obtain the original text and sends that text to the client using a call to the `IMKTextInput` protocol method `insertText(_:replacementRange:)`

## See Also

### Managing Composition

func updateComposition()

Informs the input controller that the composition has changed.

