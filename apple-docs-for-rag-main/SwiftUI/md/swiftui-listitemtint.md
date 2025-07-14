

- SwiftUI
-  ListItemTint 

Structure

# ListItemTint

A tint effect configuration that you can apply to content in a list.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
struct ListItemTint
```

## Overview

Use one of these tint values with the listItemTint(_:) view modifier. The containing list applies the tint in a platform-specific way.

## Topics

### Getting list item tint options

static let monochrome: ListItemTint

A standard grayscale tint effect.

static func fixed(Color) -> ListItemTint

An explicit tint color.

static func preferred(Color) -> ListItemTint

An explicit tint color that the system can override.

## Relationships

### Conforms To

- Sendable

## See Also

### Configuring rows

func listRowInsets(EdgeInsets?) -> some View

Applies an inset to the rows in a list.

func listRowHoverEffect(HoverEffect?) -> some View

Requests that the containing list row use the provided hover effect.

func listRowHoverEffectDisabled(Bool) -> some View

Requests that the containing list row have its hover effect disabled.

func listItemTint(_:)

Sets a fixed tint color for content in a list.

var defaultMinListRowHeight: CGFloat

The default minimum height of a row in a `List`. The default minimum height of a row in a list.

