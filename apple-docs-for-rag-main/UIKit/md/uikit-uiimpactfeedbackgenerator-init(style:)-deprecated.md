

- UIKit
- UIImpactFeedbackGenerator
-  init(style:) Deprecated

Initializer

# init(style:)

Creates an impact feedback generator with the specified style.

iOS 10.0–18.4DeprecatediPadOS 10.0–18.4DeprecatedMac Catalyst 13.1+

``` source
@MainActor
init(style: UIImpactFeedbackGenerator.FeedbackStyle)
```

Deprecated

Use init(style:view:) instead.

## Parameters 

`style`  

A value representing the mass of the colliding objects. For a list of valid feedback styles, see the UIImpactFeedbackGenerator.FeedbackStyle enumeration.

## Return Value

A newly initialized feedback generator.

## Discussion

For more information on using feedback generators, see `Using feedback generators`.

