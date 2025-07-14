

- UIKit
- UIActivityIndicatorView
-  init(style:) 

Initializer

# init(style:)

Creates an activity indicator.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(style: UIActivityIndicatorView.Style)
```

## Parameters 

`style`  

A constant that specifies the style of the object to be created. See UIActivityIndicatorView.Style for descriptions of the style constants.

## Return Value

An initialized UIActivityIndicatorView object.

## Discussion

UIActivityIndicatorView sizes the returned instance according to the specified `style`. You can set and retrieve the style of an activity indicator through the style property.

## See Also

### Creating an activity indicator

init(frame: CGRect)

Creates an activity indicator with the specified frame rectangle.

init(coder: NSCoder)

Creates an activity indicator from data in an unarchiver.

