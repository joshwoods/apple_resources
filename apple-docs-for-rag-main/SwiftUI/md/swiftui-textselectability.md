

- SwiftUI
-  TextSelectability 

Protocol

# TextSelectability

A type that describes the ability to select text.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
protocol TextSelectability
```

## Overview

To configure whether people can select text in your app, use the textSelection(_:) modifier, passing in a text selectability value like enabled or disabled.

## Topics

### Getting selectability options

static var enabled: EnabledTextSelectability

A selectability value that enables text selection by a person using your app.

static var disabled: DisabledTextSelectability

A selectability value that disables text selection by the person using your app.

### Specifying selectability

static var allowsSelection: Bool

A Boolean value that indicates whether the selectability type allows selection.

**Required**

### Supporting types

struct EnabledTextSelectability

A selectability type that enables text selection by the person using your app.

struct DisabledTextSelectability

A selectability type that disables text selection by the person using your app.

## Relationships

### Conforming Types

- DisabledTextSelectability
- EnabledTextSelectability

## See Also

### Selecting text

func textSelection&lt;S>(S) -> some View

Controls whether people can select text within this view.

struct TextSelection

Represents a selection of text.

func textSelectionAffinity(TextSelectionAffinity) -> some View

Sets the direction of a selection or cursor relative to a text character.

var textSelectionAffinity: TextSelectionAffinity

A representation of the direction or association of a selection or cursor relative to a text character. This concept becomes much more prominent when dealing with bidirectional text (text that contains both LTR and RTL scripts, like English and Arabic combined).

enum TextSelectionAffinity

A representation of the direction or association of a selection or cursor relative to a text character. This concept becomes much more prominent when dealing with bidirectional text (text that contains both LTR and RTL scripts, like English and Arabic combined).

