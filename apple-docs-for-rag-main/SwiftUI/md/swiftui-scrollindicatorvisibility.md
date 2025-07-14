

- SwiftUI
-  ScrollIndicatorVisibility 

Structure

# ScrollIndicatorVisibility

The visibility of scroll indicators of a UI element.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct ScrollIndicatorVisibility
```

## Overview

Pass a value of this type to the scrollIndicators(_:axes:) method to specify the preferred scroll indicator visibility of a view hierarchy.

## Topics

### Getting visibilties

static var automatic: ScrollIndicatorVisibility

Scroll indicator visibility depends on the policies of the component accepting the visibility configuration.

static var hidden: ScrollIndicatorVisibility

Hide the scroll indicators.

static var never: ScrollIndicatorVisibility

Scroll indicators should never be visible.

static var visible: ScrollIndicatorVisibility

Show the scroll indicators.

## Relationships

### Conforms To

- Copyable
- Equatable

## See Also

### Showing scroll indicators

func scrollIndicatorsFlash(onAppear: Bool) -> some View

Flashes the scroll indicators of a scrollable view when it appears.

func scrollIndicatorsFlash(trigger: some Equatable) -> some View

Flashes the scroll indicators of scrollable views when a value changes.

func scrollIndicators(ScrollIndicatorVisibility, axes: Axis.Set) -> some View

Sets the visibility of scroll indicators within this view.

var horizontalScrollIndicatorVisibility: ScrollIndicatorVisibility

The visibility to apply to scroll indicators of any horizontally scrollable content.

var verticalScrollIndicatorVisibility: ScrollIndicatorVisibility

The visiblity to apply to scroll indicators of any vertically scrollable content.

