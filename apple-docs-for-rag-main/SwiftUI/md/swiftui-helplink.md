

- SwiftUI
-  HelpLink 

Structure

# HelpLink

A button with a standard appearance that opens app-specific help documentation.

macOS 14.0+

``` source
struct HelpLink
```

## Overview

A help link opens documentation relevant to the context where they are used. Typically this is by opening to an anchor in an Apple Help book, but can also perform an arbitrary action such as opening a URL or opening a window.

```
HelpLink(anchor: "accountSetupHelp")

HelpLink {
    openURL(onlineHelpURL)
}
```

Help links have a standard appearance, as well as conventional placement within a view. When used within an alert or confirmation dialog’s actions, the help link will automatically be placed in the top trailing corner. Or when used in a sheet toolbar, the help link is automatically placed in the lower leading corner.

```
struct SheetContentView: View {
    var body: some View {
        Form {
             ...
        }
        .toolbar {
            ToolbarItem(.confirmationAction) {
                Button("Save") { ... }
            }
            ToolbarItem(.cancellationAction) {
                Button("Cancel") { ... }
            }
            ToolbarItem {
                HelpLink(anchor: "sheetHelp")
            }
         }
    }
}
```

## Topics

### Creating a help link

init(action: () -> Void)

Constructs a new help link with the specified action.

init(destination: URL)

Constructs a new help link that opens the specified destination URL.

init(anchor: NSHelpManager.AnchorName)

Constructs a new help link with the specified anchor in the main app bundle’s book.

init(anchor: NSHelpManager.AnchorName, book: NSHelpManager.BookName)

Constructs a new help link with the specified anchor and book.

## Relationships

### Conforms To

- View

## See Also

### Linking to other content

struct Link

A control for navigating to a URL.

struct ShareLink

A view that controls a sharing presentation.

struct SharePreview

A representation of a type to display in a share preview.

struct TextFieldLink

A control that requests text input from the user when pressed.

