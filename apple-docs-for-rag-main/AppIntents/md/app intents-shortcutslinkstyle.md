

- App Intents
-  ShortcutsLinkStyle 

Structure

# ShortcutsLinkStyle

The styles to apply to buttons you use to open your app’s page in the Shortcuts app.

AppIntentsSwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
struct ShortcutsLinkStyle
```

## Overview

Specify a ShortcutsLinkStyle value when you add a ShortcutsUIButton or ShortcutsLink type to your interface. For the ShortcutsLink type, specify the style using the shortcutsLinkStyle(_:) modifier.

## Topics

### Getting the styles

static let automatic: ShortcutsLinkStyle

The default button style, based on the current color scheme.

static let automaticOutline: ShortcutsLinkStyle

The default button style with an outline, based on the current color scheme.

### Type Properties

static let dark: ShortcutsLinkStyle

A button style that applies a dark background with light text.

static let darkOutline: ShortcutsLinkStyle

A button style that applies a dark background with light text along with a light outline.

static let light: ShortcutsLinkStyle

A button style that applies a light background with dark text.

static let lightOutline: ShortcutsLinkStyle

A button style that applies a light background with dark text along with a dark outline.

## See Also

### Buttons

class ShortcutsUIButton

A button that opens the current app’s page in the Shortcuts app.

struct ShortcutsLink

A button that brings users to the current app’s App Shortcuts page in the Shortcuts app.

