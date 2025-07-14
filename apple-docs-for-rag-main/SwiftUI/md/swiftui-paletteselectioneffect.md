

- SwiftUI
-  PaletteSelectionEffect 

Structure

# PaletteSelectionEffect

The selection effect to apply to a palette item.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
struct PaletteSelectionEffect
```

## Overview

You can configure the selection effect of a palette item by using the paletteSelectionEffect(_:) view modifier.

## Topics

### Getting palette selection effects

static let automatic: PaletteSelectionEffect

Applies the system’s default effect when selected.

static let custom: PaletteSelectionEffect

Does not apply any system effect when selected.

static func symbolVariant(SymbolVariants) -> PaletteSelectionEffect

Applies the specified symbol variant when selected.

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Choosing from a set of options

struct Picker

A control for selecting from a set of mutually exclusive values.

func pickerStyle&lt;S>(S) -> some View

Sets the style for pickers within this view.

func horizontalRadioGroupLayout() -> some View

Sets the style for radio group style pickers within this view to be horizontally positioned with the radio buttons inside the layout.

func defaultWheelPickerItemHeight(CGFloat) -> some View

Sets the default wheel-style picker item height.

var defaultWheelPickerItemHeight: CGFloat

The default height of an item in a wheel-style picker, such as a date picker.

func paletteSelectionEffect(PaletteSelectionEffect) -> some View

Specifies the selection effect to apply to a palette item.

