

- UIKit
- UIResponderStandardEditActions
-  selectAll(\_:) 

Instance Method

# selectAll(\_:)

Selects all of the content in the current responder.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func selectAll(_ sender: Any?)
```

## Parameters 

`sender`  

The object calling this method.

## Discussion

UIKit calls this method when the user selects the Select All command from an editing menu. The command selects all content in the responder. For example, a text view selects all of its text and displays an appropriate selection interface.

## See Also

### Handling selection commands

func select(Any?)

Selects the content in your responder.

