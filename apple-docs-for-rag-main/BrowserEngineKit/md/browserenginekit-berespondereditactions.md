

- BrowserEngineKit
-  BEResponderEditActions 

Protocol

# BEResponderEditActions

A set of methods that defines extended interactions in browser text views.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
protocol BEResponderEditActions : UIResponderStandardEditActions
```

## Mentioned in 

Supporting extended text interactions

## Overview

Implement the methods in this protocol to support text interactions in your browser text view that conforms to BETextInput. To get the operating system’s standard behavior for an interaction, call BETextInteraction methods in your implementation. For more information, see Supporting extended text interactions.

## Topics

### Finding and replacing text

func findSelected(Any?)

Begins a search for the selected content in your browser text view.

func promptForReplace(Any?)

Shows potential replacements for the selected content.

func replace(Any?)

Removes the selected text and inputs the chosen replacement text.

func addShortcut(Any?)

Adds a text-replacement shortcut to the edit dictionary.

### Defining and sharing text

func lookup(Any?)

Presents a dictionary definition for the selected content.

func share(Any?)

Presents UI for sharing the selected text.

### Translating and transliterating text

func translate(Any?)

Presents a translation of the selected text.

func transliterateChinese(Any?)

Converts the selected text between traditional and simplified Chinese.

## Relationships

### Inherits From

- NSObjectProtocol
- UIResponderStandardEditActions

### Inherited By

- BETextInput

## See Also

### Interaction responses

class BETextInteraction

An interaction you add to a text view to support extended text gestures.

protocol BETextInteractionDelegate

A set of methods that informs you about selection changes in text views.

enum BEGestureType

