

- UIKit
- UIButton
-  init(coder:) 

Initializer

# init(coder:)

Creates a new button with data in an unarchiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init?(coder: NSCoder)
```

## Parameters 

`coder`  

An unarchiver object.

## See Also

### Creating buttons

init(frame: CGRect)

Creates a new button with the specified frame.

convenience init(frame: CGRect, primaryAction: UIAction?)

Creates a new button with the specified frame, registers the primary action event, and sets the title and image to the action’s title and image.

