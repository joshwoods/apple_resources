

- UIKit
-  Handwriting recognition 

API Collection

# Handwriting recognition

Configure text fields and custom views that accept text to handle input from Apple Pencil.

## Topics

### Essentials

Customizing Scribble with Interactions

Enable writing on a non-text-input view by adding interactions.

### Text fields

class UIScribbleInteraction

An interaction for customizing the behavior of Scribble on text input views, or for suppressing it entirely in specific cases.

protocol UIScribbleInteractionDelegate

Methods for customizing or suppressing Scribble behavior within text input views.

### Custom views

class UIIndirectScribbleInteraction

An interaction for using Scribble to enter text by writing on a view that isn’t formally a text input.

protocol UIIndirectScribbleInteractionDelegate

Methods that customize behavior on views that aren’t formally text input views.

associatedtype ElementIdentifier : Hashable = String

A unique identifier for a control that isn’t a text field in a Scribble interaction.

**Required**

## See Also

### Text

Text display and fonts

Display text, manage fonts, and check spelling.

TextKit

Manage text storage and perform custom layout of text-based content in your app’s views.

Keyboards and input

Configure the system keyboard, create your own keyboards to handle input, or detect key presses on a physical keyboard.

Writing Tools

Add support for Writing Tools to your app’s text views.

