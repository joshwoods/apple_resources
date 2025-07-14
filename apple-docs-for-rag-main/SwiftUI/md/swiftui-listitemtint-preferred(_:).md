

- SwiftUI
- ListItemTint
-  preferred(\_:) 

Type Method

# preferred(\_:)

An explicit tint color that the system can override.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static func preferred(_ tint: Color) -> ListItemTint
```

## Parameters 

`tint`  

The color to use to tint the content.

## Discussion

The system can override this tint effect, like when the system has a custom user accent color on macOS.

## See Also

### Getting list item tint options

static let monochrome: ListItemTint

A standard grayscale tint effect.

static func fixed(Color) -> ListItemTint

An explicit tint color.

