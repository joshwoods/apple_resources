

- SwiftUI
- KeyboardShortcut
-  KeyboardShortcut.Localization 

Structure

# KeyboardShortcut.Localization

Options for how a keyboard shortcut participates in automatic localization.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
struct Localization
```

## Overview

A shortcut’s `key` that is defined on an US-English keyboard layout might not be reachable on international layouts. For example the shortcut `⌘[` works well for the US layout but is hard to reach for German users. On the German keyboard layout, pressing `⌥5` will produce `[`, which causes the shortcut to become `⌥⌘5`. If configured, which is the default behavior, automatic shortcut remapping will convert it to `⌘Ö`.

In addition to that, some keyboard shortcuts carry information about directionality. Right-aligning a block of text or seeking forward in context of music playback are such examples. These kinds of shortcuts benefit from the option withoutMirroring to tell the system that they won’t be flipped when running in a right-to-left context.

## Topics

### Getting localization strategies

static let automatic: KeyboardShortcut.Localization

Remap shortcuts to their international counterparts, mirrored for right-to-left usage if appropriate.

static let custom: KeyboardShortcut.Localization

Don’t use automatic shortcut remapping.

static let withoutMirroring: KeyboardShortcut.Localization

Don’t mirror shortcuts.

## Relationships

### Conforms To

- Sendable

## See Also

### Creating a localized shortcut

init(KeyEquivalent, modifiers: EventModifiers, localization: KeyboardShortcut.Localization)

Creates a new keyboard shortcut with the given key equivalent and set of modifier keys.

var localization: KeyboardShortcut.Localization

The localization strategy to apply to this shortcut.

