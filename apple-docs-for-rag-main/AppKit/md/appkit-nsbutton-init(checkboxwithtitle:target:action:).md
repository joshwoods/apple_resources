

- AppKit
- NSButton
-  init(checkboxWithTitle:target:action:) 

Initializer

# init(checkboxWithTitle:target:action:)

Creates a standard checkbox with the title you specify.

macOS 10.12+

``` source
@MainActor
convenience init(
    checkboxWithTitle title: String,
    target: Any?,
    action: Selector?
)
```

## Parameters 

`title`  

The localized title string to display on the button.

`target`  

The target object that receives action messages from the button.

`action`  

The action message the button sends to the target.

## See Also

### Creating Standard Buttons

convenience init(image: NSImage, target: Any?, action: Selector?)

Creates a standard push button with the image you specify.

convenience init(radioButtonWithTitle: String, target: Any?, action: Selector?)

Creates a standard radio button with the title you specify.

convenience init(title: String, image: NSImage, target: Any?, action: Selector?)

Creates a standard push button with a title and image.

convenience init(title: String, target: Any?, action: Selector?)

Creates a standard push button with the title you specify.

