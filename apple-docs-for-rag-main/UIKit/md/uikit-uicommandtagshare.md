

- UIKit
-  UICommandTagShare 

Global Variable

# UICommandTagShare

A value that identifies a command as a Share menu.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
let UICommandTagShare: String
```

## Discussion

To create a Share menu, add UICommandTagShare to the `propertyList` of a UICommand or UIKeyCommand object.

```
// Ensure that the builder is modifying the menu bar system.
guard builder.system == UIMenuSystem.main else { return }

let shareCommand = UICommand(title: "Share",
                             action: #selector(share(_:)),
                             propertyList: UICommandTagShare)

let shareMenu = UIMenu(title: "", options: .displayInline, children: [shareCommand])

// Insert the menu into the File menu before the Close menu.
builder.insertSibling(shareMenu, beforeMenu: .close)
```

## See Also

### Associating data

var propertyList: Any?

An object that contains data to associate with the command.

