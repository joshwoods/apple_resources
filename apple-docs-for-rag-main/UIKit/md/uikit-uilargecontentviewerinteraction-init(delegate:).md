

- UIKit
- UILargeContentViewerInteraction
-  init(delegate:) 

Initializer

# init(delegate:)

Creates an interaction object with the specified delegate.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init(delegate: (any UILargeContentViewerInteractionDelegate)?)
```

## Parameters 

`delegate`  

An object that implements the UILargeContentViewerInteractionDelegate protocol.

## Discussion

To add the interaction to a view, use addInteraction(_:).

