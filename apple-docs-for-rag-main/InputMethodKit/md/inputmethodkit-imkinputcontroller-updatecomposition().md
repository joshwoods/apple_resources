

- InputMethodKit
- IMKInputController
-  updateComposition() 

Instance Method

# updateComposition()

Informs the input controller that the composition has changed.

macOS 10.5+

``` source
func updateComposition()
```

## Discussion

This method calls the protocol method composedString: to obtain the current composition. The current composition is sent to the client by a call to the method `setMarkedText(_:selectionRange:replacementRange:)`.

## See Also

### Managing Composition

func cancelComposition()

Stops the current composition and replaces marked text with the original text.

