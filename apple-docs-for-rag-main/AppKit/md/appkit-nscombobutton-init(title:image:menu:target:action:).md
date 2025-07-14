

- AppKit
- NSComboButton
-  init(title:image:menu:target:action:) 

Initializer

# init(title:image:menu:target:action:)

Creates a combo button that displays both a title and image.

macOS 13.0+

``` source
@MainActor
convenience init(
    title: String,
    image: NSImage,
    menu: NSMenu?,
    target: Any?,
    action: Selector?
)
```

## Parameters 

`title`  

The localized string to display in the button. Use the inherited alignment property to set the text alignment for the string.

`image`  

The image to display in the button.

`menu`  

The menu to display when someone chooses an alternate action.

`target`  

The object that receives the default action message when someone clicks the button.

`action`  

The action message to send to the `target` object.

## Return Value

A combo button configured with both a title and image.

## See Also

### Creating a Combo Button

convenience init(title: String, menu: NSMenu?, target: Any?, action: Selector?)

Creates a combo button that displays a title.

convenience init(image: NSImage, menu: NSMenu?, target: Any?, action: Selector?)

Creates a combo button that displays an image.

