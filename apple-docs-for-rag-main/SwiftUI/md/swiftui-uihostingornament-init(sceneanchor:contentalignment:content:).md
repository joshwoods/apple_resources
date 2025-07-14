

- SwiftUI
- UIHostingOrnament
-  init(sceneAnchor:contentAlignment:content:) 

Initializer

# init(sceneAnchor:contentAlignment:content:)

Creates an ornament with the specified alignment and content.

visionOS 1.0+

``` source
init(
    sceneAnchor: UnitPoint,
    contentAlignment: Alignment = .center,
    @ViewBuilder content: () -> Content
)
```

## Parameters 

`sceneAnchor`  

The anchor point for aligning the ornament’s content (based on the `contentAlignment`) with the scene.

`contentAlignment`  

The alignment in the ornament used to position it.

`content`  

The content of the ornament.

