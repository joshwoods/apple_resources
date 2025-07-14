

- AppKit
- NSResponder
-  noResponder(for:) 

Instance Method

# noResponder(for:)

Handles the case where an event or action message falls off the end of the responder chain.

macOS

``` source
@MainActor
func noResponder(for eventSelector: Selector)
```

## Parameters 

`eventSelector`  

A selector identifying the action or event message.

## Discussion

The default implementation beeps if `eventSelector` is keyDown(with:).

