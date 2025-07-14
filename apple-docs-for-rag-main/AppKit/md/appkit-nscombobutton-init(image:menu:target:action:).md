

- AppKit
- NSComboButton
-  init(image:menu:target:action:) 

Initializer

# init(image:menu:target:action:)

Creates a combo button that displays an image.

macOS 13.0+

``` source
@MainActor
convenience init(
    image: NSImage,
    menu: NSMenu?,
    target: Any?,
    action: Selector?
)
```

## Parameters 

`image`  

The image to display in the button.

`menu`  

The menu to display when someone chooses an alternate action.

`target`  

The object that receives the default action message when someone clicks the button.

`action`  

The action message to send to the `target` object.

## Return Value

A combo button configured with only the specified image.

## Discussion

This method sets the title property to an empty string.

## See Also

### Creating a Combo Button

convenience init(title: String, image: NSImage, menu: NSMenu?, target: Any?, action: Selector?)

Creates a combo button that displays both a title and image.

convenience init(title: String, menu: NSMenu?, target: Any?, action: Selector?)

Creates a combo button that displays a title.

