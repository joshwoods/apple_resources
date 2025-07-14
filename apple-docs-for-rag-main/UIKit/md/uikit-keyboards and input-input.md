

- UIKit
-  Keyboards and input 

API Collection

# Keyboards and input

Configure the system keyboard, create your own keyboards to handle input, or detect key presses on a physical keyboard.

## Topics

### Text input

protocol UITextInput

A set of methods for interacting with the text input system and enabling features in documents.

protocol UITextInputDelegate

An intermediary between a document and the text input system.

protocol UIKeyInput

A set of methods a responder uses to implement simple text entry.

protocol UITextInputTraits

A set of methods that defines features for keyboard input to a text object.

class UITextInputContext

An object that reports the type of input your app receives.

class UITextInputMode

The current text input mode.

class UITextInputAssistantItem

An object that manages custom bar button items that you add to the shortcuts bar above the keyboard on iPad.

class UIDictationPhrase

An object that represents the textual interpretation of a spoken phrase that the user dictates.

### Text interactions

class UITextInteraction

An interaction that provides text selection gestures and UI to custom text views.

protocol UITextInteractionDelegate

An interface that an object implements to receive information about text interaction events.

enum UITextInteractionMode

Modes that determine the selection behaviors that a text interaction provides.

### Custom text selection

Adopting system selection UI in custom text views

Incorporate the system text-selection experience into your custom text UI in UIKit.

class UITextSelectionDisplayInteraction

An object that provides the system UI for displaying text selection.

protocol UITextSelectionHighlightView

An interface you use to provide a custom highlight UI behind the selected text.

protocol UITextSelectionHandleView

An interface you use to draw custom the selection handles for ranges of text.

protocol UITextCursorView

An interface you use to draw the insertion point in a piece of text.

class UIStandardTextCursorView

A view that draws the standard system insertion point in a piece of text.

class UITextCursorDropPositionAnimator

class UITextLoupeSession

An object that manages the presentation of the system magnifier at the location you specify.

### Text actions and menus

class UITextItem

An object for attaching custom actions and menus to links, text attachments, or other specific text in a text view.

class MenuConfiguration

An object that describes what type of menu and preview to show for a text item.

protocol UITextViewDelegate

The methods for receiving editing-related messages for text view objects.

### Smart Reply for messaging

Adopting Smart Reply in your messaging or email app

Generate reply suggestions by using Apple Intelligence and put selected text into your text UI.

class UIConversationContext

A base class that represents a conversation between participants, such as in an email or messaging app.

class Entry

A base class that represents a message in a conversation.

class UIMailConversationContext

A class that represents an email conversation.

class MailEntry

A class that represents a specific email in an email thread.

class UIMessageConversationContext

A class that represents a message conversation.

class MessageEntry

A class that represents a message in a message conversation.

class UIInputSuggestion

A base class you use to handle suggestions from the keyboard or system.

class UISmartReplySuggestion

A class you use to handle a Smart Reply suggestion.

### Text tokenizer

protocol UITextInputTokenizer

A tokenizer, which is an object that allows the text input system to evaluate text units of different granularities.

class UITextInputStringTokenizer

A base implementation of the text-input tokenizer protocol.

### Keyboard layout

Adjusting your layout with keyboard layout guide

Respond dynamically to keyboard movement by using the tracking features of the keyboard layout guide.

class UIKeyboardLayoutGuide

A layout guide that represents the space the keyboard occupies in your app’s layout.

class UITrackingLayoutGuide

A layout guide that automatically activates and deactivates layout constraints depending on its proximity to edges.

### Custom keyboards

Creating a custom keyboard

Add an extension to your Xcode project to provide systemwide customized text input.

class UIInputViewController

The primary view controller for a custom keyboard app extension.

class UIInputView

An object that displays and manages custom input for a view when that view becomes the first responder.

class UILexicon

A read-only array of term pairs, each in a lexicon entry object, for a custom keyboard.

class UILexiconEntry

A read-only term pair, available within a lexicon object, for a custom keyboard.

protocol UITextDocumentProxy

An object that provides textual context to a custom keyboard.

### Physical keyboards

Handling key presses made on a physical keyboard

Detect when someone presses and releases keys on a physical keyboard.

Navigating an app’s user interface using a keyboard

Navigate between user interface elements using a keyboard and focusable UI elements in iPad apps and apps built with Mac Catalyst.

Adding hardware keyboard support to your app

Enhance interactions with your app by handling raw keyboard events, writing custom keyboard shortcuts, and working with gesture recognizers.

class UIKey

An object that provides information about the state of a keyboard key.

enum UIKeyboardHIDUsage

A set of HID usage codes that identify the keys of a USB keyboard.

## See Also

### Text

Text display and fonts

Display text, manage fonts, and check spelling.

TextKit

Manage text storage and perform custom layout of text-based content in your app’s views.

Writing Tools

Add support for Writing Tools to your app’s text views.

Handwriting recognition

Configure text fields and custom views that accept text to handle input from Apple Pencil.

