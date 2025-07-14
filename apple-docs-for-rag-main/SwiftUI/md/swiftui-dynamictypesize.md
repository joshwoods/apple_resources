

- SwiftUI
-  DynamicTypeSize 

Enumeration

# DynamicTypeSize

A Dynamic Type size, which specifies how large scalable content should be.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum DynamicTypeSize
```

## Overview

For more information, see Typography in the Human Interface Guidelines.

## Topics

### Getting type sizes

case xSmall

An extra small size.

case small

A small size.

case medium

A medium size.

case large

A large size.

case xLarge

An extra large size.

case xxLarge

An extra extra large size.

case xxxLarge

An extra extra extra large size.

### Getting accessibility type sizes

case accessibility1

The first accessibility size.

case accessibility2

The second accessibility size.

case accessibility3

The third accessibility size.

case accessibility4

The fourth accessibility size.

case accessibility5

The fifth accessibility size.

var isAccessibilitySize: Bool

A Boolean value indicating whether the size is one that is associated with accessibility.

### Creating a type size

init?(UIContentSizeCategory)

Create a Dynamic Type size from its `UIContentSizeCategory` equivalent.

## Relationships

### Conforms To

- CaseIterable
- Comparable
- Equatable
- Hashable
- Sendable

## See Also

### Adjusting text size

func textScale(Text.Scale, isEnabled: Bool) -> some View

Applies a text scale to text in the view.

func dynamicTypeSize(_:)

Sets the Dynamic Type size within the view to the given value.

var dynamicTypeSize: DynamicTypeSize

The current Dynamic Type size.

struct ScaledMetric

A dynamic property that scales a numeric value.

protocol TextVariantPreference

A protocol for controlling the size variant of text views.

struct FixedTextVariant

The default text variant preference that chooses the largest available variant.

struct SizeDependentTextVariant

The size dependent variant preference allows the text to take the available space into account when choosing the variant to display.

