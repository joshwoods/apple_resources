

- AppKit
- NSResponder
-  nextResponder 

Instance Property

# nextResponder

The next responder after this one, or `nil` if it has none.

macOS

``` source
@MainActor
unowned(unsafe) var nextResponder: NSResponder? { get set }
```

## Discussion

The next responder must be an object that inherits, directly or indirectly, from `NSResponder`.

## See Also

### Related Documentation

func noResponder(for: Selector)

Handles the case where an event or action message falls off the end of the responder chain.

