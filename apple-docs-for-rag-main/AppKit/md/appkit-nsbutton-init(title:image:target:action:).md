

- AppKit
- NSButton
-  init(title:image:target:action:) 

Initializer

# init(title:image:target:action:)

Creates a standard push button with a title and image.

macOS 10.12+

``` source
@MainActor
convenience init(
    title: String,
    image: NSImage,
    target: Any?,
    action: Selector?
)
```

## Parameters 

`title`  

The localized title string to display on the button.

`image`  

The image to display in the body of the button.

`target`  

The target object that receives action messages from the button.

`action`  

The action message the button sends to the target.

## See Also

### Creating Standard Buttons

convenience init(checkboxWithTitle: String, target: Any?, action: Selector?)

Creates a standard checkbox with the title you specify.

convenience init(image: NSImage, target: Any?, action: Selector?)

Creates a standard push button with the image you specify.

convenience init(radioButtonWithTitle: String, target: Any?, action: Selector?)

Creates a standard radio button with the title you specify.

convenience init(title: String, target: Any?, action: Selector?)

Creates a standard push button with the title you specify.

