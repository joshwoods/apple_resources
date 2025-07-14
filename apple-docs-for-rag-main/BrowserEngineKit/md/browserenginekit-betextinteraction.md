

- BrowserEngineKit
-  BETextInteraction 

Class

# BETextInteraction

An interaction you add to a text view to support extended text gestures.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
class BETextInteraction
```

## Mentioned in 

Supporting extended text interactions

Integrating custom browser text views with UIKit

## Overview

Add a `BETextInteraction` object to your browser text view’s textInputView. When your browser text view receives text-interaction actions, call the methods on this object to invoke the standard operating system behavior.

## Topics

### Text selection

var delegate: (any BETextInteractionDelegate)?

A delegate object that the interaction notifies when the system changes the text selection.

protocol BETextInteractionDelegate

A set of methods that informs you about selection changes in text views.

var textSelectionDisplayInteraction: UITextSelectionDisplayInteraction

An interaction that manages the system’s text-selection UI.

func selectionBoundaryAdjusted(to: CGPoint, touchPhase: BESelectionTouchPhase, flags: BESelectionFlags)

Notifies the system after the text view adjusts its selection.

func selectionChangedWithGesture(at: CGPoint, gesture: BEGestureType, state: UIGestureRecognizer.State, flags: BESelectionFlags)

Notifies the system that the text view changed its selection.

### Menus

func presentEditMenuForSelection()

Presents an edit menu for the current text selection.

func dismissEditMenuForSelection()

Dismisses the edit menu for the current text selection.

var contextMenuInteraction: UIContextMenuInteraction

An interaction you use to work with the text view’s context menu.

var contextMenuInteractionDelegate: (any UIContextMenuInteractionDelegate)?

The delegate for the context menu interaction associated with this text interaction.

### Text replacements

func addShortcut(forText: String, from: CGRect)

Presents UI for a person to add a text-replacement shortcut to the keyboard dictionary.

func showReplacements(forText: String)

Displays inline text replacements for the current selection.

### Sharing and defining text

func share(text: String, from: CGRect)

Presents standard UI for someone to share text from a browser text view.

func showDictionary(forTextInContext: String, definingTextInRange: NSRange, from: CGRect)

Presents a dictionary definition for the supplied text.

### Translation and transliteration

func translate(text: String, from: CGRect)

Presents a translation of the text.

func transliterateChinese(forText: String)

Converts the text between traditional and simplified Chinese.

### UI updates

func editabilityChanged()

Tells the system that the document’s editability status has changed.

func refreshKeyboardUI()

Tells the system to refresh the keyboard UI.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable
- UIInteraction

## See Also

### Interaction responses

protocol BETextInteractionDelegate

A set of methods that informs you about selection changes in text views.

protocol BEResponderEditActions

A set of methods that defines extended interactions in browser text views.

enum BEGestureType

protocol BEResponderEditActions

A set of methods that defines extended interactions in browser text views.

