

- UIKit
- UIDropInteraction
-  init(delegate:) 

Initializer

# init(delegate:)

Initializes a drop interaction object with a custom delegate object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init(delegate: any UIDropInteractionDelegate)
```

## Parameters 

`delegate`  

An object that conforms to the UIDropInteractionDelegate protocol.

## Return Value

A drop interaction that has a delegate.

