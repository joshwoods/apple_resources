

- SwiftUI
-  NavigationBarItem 

Structure

# NavigationBarItem

A configuration for a navigation bar that represents a view at the top of a navigation stack.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct NavigationBarItem
```

## Overview

Use one of the NavigationBarItem.TitleDisplayMode values to configure a navigation bar title’s display mode with the navigationBarTitleDisplayMode(_:) view modifier.

## Topics

### Setting a title display mode

enum TitleDisplayMode

A style for displaying the title of a navigation bar.

## Relationships

### Conforms To

- Sendable

## See Also

### Configuring the navigation bar

func navigationBarBackButtonHidden(Bool) -> some View

Hides the navigation bar back button for the view.

func navigationBarTitleDisplayMode(NavigationBarItem.TitleDisplayMode) -> some View

Configures the title display mode for this view.

