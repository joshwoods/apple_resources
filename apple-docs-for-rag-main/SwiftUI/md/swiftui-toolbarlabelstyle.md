

- SwiftUI
-  ToolbarLabelStyle 

Structure

# ToolbarLabelStyle

The label style of a toolbar.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct ToolbarLabelStyle
```

## Overview

Use this type in conjunction with modifiers like windowToolbarLabelStyle(fixed:) and windowToolbarLabelStyle(_:) to customize the appearance of window toolbars managed by SwiftUI.

## Topics

### Type Properties

static var automatic: ToolbarLabelStyle

The automatic label style. The toolbar will use a labelStyle that best fits the `Scene` it is applied to.

static var iconOnly: ToolbarLabelStyle

The icon only label style. The toolbar contents will only display the control

static var titleAndIcon: ToolbarLabelStyle

The title and icon label style. The toolbar contents will display both a control and title

static var titleOnly: ToolbarLabelStyle

The title only label style. The toolbar contents will only display the title

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Styling a toolbar

func toolbarBackground(_:for:)

Specifies the preferred shape style of the background of a bar managed by SwiftUI.

func toolbarColorScheme(ColorScheme?, for: ToolbarPlacement...) -> some View

Specifies the preferred color scheme of a bar managed by SwiftUI.

func toolbarForegroundStyle&lt;S>(S, for: ToolbarPlacement...) -> some View

Specifies the preferred foreground style of bars managed by SwiftUI.

func windowToolbarStyle&lt;S>(S) -> some Scene

Sets the style for the toolbar defined within this scene.

protocol WindowToolbarStyle

A specification for the appearance and behavior of a window’s toolbar.

var toolbarLabelStyle: ToolbarLabelStyle?

The label style to apply to controls within a toolbar.

