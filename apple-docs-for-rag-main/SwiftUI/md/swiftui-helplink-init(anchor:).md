

- SwiftUI
- HelpLink
-  init(anchor:) 

Initializer

# init(anchor:)

Constructs a new help link with the specified anchor in the main app bundle’s book.

macOS 14.0+

``` source
init(anchor: NSHelpManager.AnchorName)
```

## Parameters 

`anchor`  

The anchor within the help book to open to.

## Discussion

The main app bundle book name is defined by the `CFBundleHelpBookName` key in its Info.plist file.

## See Also

### Creating a help link

init(action: () -> Void)

Constructs a new help link with the specified action.

init(destination: URL)

Constructs a new help link that opens the specified destination URL.

init(anchor: NSHelpManager.AnchorName, book: NSHelpManager.BookName)

Constructs a new help link with the specified anchor and book.

