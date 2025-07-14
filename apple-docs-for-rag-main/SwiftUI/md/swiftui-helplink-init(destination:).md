

- SwiftUI
- HelpLink
-  init(destination:) 

Initializer

# init(destination:)

Constructs a new help link that opens the specified destination URL.

macOS 14.0+

``` source
init(destination: URL)
```

## Parameters 

`destination`  

The URL to open when the button is clicked.

## Discussion

Use this initializer when you want the standard help button appearance that opens a link to a website.

You can override the default behavior when the button is clicked by setting the openURL environment value with a custom OpenURLAction.

## See Also

### Creating a help link

init(action: () -> Void)

Constructs a new help link with the specified action.

init(anchor: NSHelpManager.AnchorName)

Constructs a new help link with the specified anchor in the main app bundle’s book.

init(anchor: NSHelpManager.AnchorName, book: NSHelpManager.BookName)

Constructs a new help link with the specified anchor and book.

