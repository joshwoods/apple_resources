

- UIKit
- UIResponderStandardEditActions
-  select(\_:) 

Instance Method

# select(\_:)

Selects the content in your responder.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func select(_ sender: Any?)
```

## Parameters 

`sender`  

The object calling this method.

## Discussion

UIKit calls this method when the user selects the Select command from an editing menu. The command is used for the targeted selection of content in a view. For example, a text view uses this to select one or more words in the view and to display the selection interface.

## See Also

### Handling selection commands

func selectAll(Any?)

Selects all of the content in the current responder.

