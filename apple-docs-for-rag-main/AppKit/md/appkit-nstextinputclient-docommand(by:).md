

- AppKit
- NSTextInputClient
-  doCommand(by:) 

Instance Method

# doCommand(by:)

Invokes the action specified by the given selector.

macOS 10.0+

``` source
func doCommand(by selector: Selector)
```

**Required**

## Parameters 

`selector`  

The selector to invoke.

## Discussion

If `selector` cannot be invoked, then `doCommandBySelector:` should not pass this message up the responder chain. `NSResponder` also implements this method, and it does forward uninvokable commands up the responder chain, but a text view should not. A text view implementing the `NSTextInputClient` protocol inherits from `NSView`, which inherits from `NSResponder`, so your implementation of this method will override the one in `NSResponder`. It should not call `super`.

## See Also

### Related Documentation

func interpretKeyEvents([NSEvent])

Handles a series of key events.

