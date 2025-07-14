

- SwiftUI
- HelpLink
-  init(action:) 

Initializer

# init(action:)

Constructs a new help link with the specified action.

macOS 14.0+

``` source
init(action: @escaping () -> Void)
```

## Parameters 

`action`  

The action to perform when the user clicks the button.

## Discussion

Use this initializer when you want the standard help button appearance with a custom button action that does not open an article in an Apple Help book.

## See Also

### Creating a help link

init(destination: URL)

Constructs a new help link that opens the specified destination URL.

init(anchor: NSHelpManager.AnchorName)

Constructs a new help link with the specified anchor in the main app bundle’s book.

init(anchor: NSHelpManager.AnchorName, book: NSHelpManager.BookName)

Constructs a new help link with the specified anchor and book.

