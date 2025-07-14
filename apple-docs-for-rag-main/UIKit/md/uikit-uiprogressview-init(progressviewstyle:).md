

- UIKit
- UIProgressView
-  init(progressViewStyle:) 

Initializer

# init(progressViewStyle:)

Creates a progress view with the specified style.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
convenience init(progressViewStyle style: UIProgressView.Style)
```

## Parameters 

`style`  

A constant that specifies the style of the object to be created. See UIProgressView.Style for descriptions of the style constants.

## Return Value

An initialized UIProgressView object.

## Discussion

UIProgressView sets the height of the returned view according to the specified `style`. You can set and retrieve the style of a progress view through the progressViewStyle property.

## See Also

### Creating a progress view

init(frame: CGRect)

Creates a progress view with the specified frame rectangle.

init?(coder: NSCoder)

Creates a progress view from data in an unarchiver.

