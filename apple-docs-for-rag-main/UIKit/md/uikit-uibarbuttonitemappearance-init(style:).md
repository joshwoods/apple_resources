

- UIKit
- UIBarButtonItemAppearance
-  init(style:) 

Initializer

# init(style:)

Creates an appearance with default values that are appropriate for the specified button style.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
init(style: UIBarButtonItem.Style)
```

## Parameters 

`style`  

The button style. UIKit uses this value to configure the default appearance attributes. For a list of possible values, see UIBarButtonItem.Style.

## Return Value

A new bar button item appearance object containing the default appearances for the specified button style.

## See Also

### Creating a bar button item appearance object

convenience init()

Creates an appearance object with default values that are appropriate for a plain button.

init(coder: NSCoder)

Creates an appearance object from data in an unarchiver.

