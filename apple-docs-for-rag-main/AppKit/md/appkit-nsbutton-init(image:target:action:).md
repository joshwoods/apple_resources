

- AppKit
- NSButton
-  init(image:target:action:) 

Initializer

# init(image:target:action:)

Creates a standard push button with the image you specify.

macOS 10.12+

``` source
@MainActor
convenience init(
    image: NSImage,
    target: Any?,
    action: Selector?
)
```

## Parameters 

`image`  

The image to display in the body of the button.

`target`  

The target object that receives action messages from the button.

`action`  

The action message the button sends to the target.

## Discussion

Set the image’s accessibilityDescription property to ensure accessibility for this control.

## See Also

### Creating Standard Buttons

convenience init(checkboxWithTitle: String, target: Any?, action: Selector?)

Creates a standard checkbox with the title you specify.

convenience init(radioButtonWithTitle: String, target: Any?, action: Selector?)

Creates a standard radio button with the title you specify.

convenience init(title: String, image: NSImage, target: Any?, action: Selector?)

Creates a standard push button with a title and image.

convenience init(title: String, target: Any?, action: Selector?)

Creates a standard push button with the title you specify.

