

- SwiftUI
- HelpLink
-  init(anchor:book:) 

Initializer

# init(anchor:book:)

Constructs a new help link with the specified anchor and book.

macOS 14.0+

``` source
init(
    anchor: NSHelpManager.AnchorName,
    book: NSHelpManager.BookName
)
```

## Parameters 

`anchor`  

The anchor within the help book to open to.

`book`  

The specific book name to open.

## See Also

### Creating a help link

init(action: () -> Void)

Constructs a new help link with the specified action.

init(destination: URL)

Constructs a new help link that opens the specified destination URL.

init(anchor: NSHelpManager.AnchorName)

Constructs a new help link with the specified anchor in the main app bundle’s book.

