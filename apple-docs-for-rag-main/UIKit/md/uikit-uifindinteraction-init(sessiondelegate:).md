

- UIKit
- UIFindInteraction
-  init(sessionDelegate:) 

Initializer

# init(sessionDelegate:)

Initializes a find interaction object with the delegate object you specify.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
init(sessionDelegate: any UIFindInteractionDelegate)
```

## Return Value

Returns a find interaction object with the associated delegate.

## Discussion

Create an object that conforms to the UIFindInteractionDelegate protocol and assign it to this property.

