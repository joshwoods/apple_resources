

- SwiftUI
- ListItemTint
-  fixed(\_:) 

Type Method

# fixed(\_:)

An explicit tint color.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static func fixed(_ tint: Color) -> ListItemTint
```

## Parameters 

`tint`  

The color to use to tint the content.

## Discussion

The system doesn’t override this tint effect.

## See Also

### Getting list item tint options

static let monochrome: ListItemTint

A standard grayscale tint effect.

static func preferred(Color) -> ListItemTint

An explicit tint color that the system can override.

