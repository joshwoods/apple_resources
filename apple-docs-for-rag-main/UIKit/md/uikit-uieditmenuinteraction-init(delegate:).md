

- UIKit
- UIEditMenuInteraction
-  init(delegate:) 

Initializer

# init(delegate:)

Initializes an edit menu interaction object with the delegate object you specify.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
init(delegate: (any UIEditMenuInteractionDelegate)?)
```

## Discussion

Create an object that conforms to the UIEditMenuInteractionDelegate protocol and assign it to this property. The interaction uses the system delegate if no delegate is provided (if you pass in `nil`).

