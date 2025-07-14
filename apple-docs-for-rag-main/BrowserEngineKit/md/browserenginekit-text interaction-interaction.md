

- BrowserEngineKit
-  Text interaction 

API Collection

# Text interaction

Integrate your web browser engine asynchronously with the text system.

## Topics

### Custom text views

Integrating custom browser text views with UIKit

Process keyboard interactions asynchronously in your iOS browser app’s text view.

Supporting extended text interactions

Share content, add replacement shortcuts, and perform other rich actions in browser text views.

protocol BETextInput

A protocol to which text views conform to asynchronously integrate with the text system.

protocol BETextInputDelegate

A delegate protocol that a browser text view uses to notify the text system of changes.

### Interaction responses

class BETextInteraction

An interaction you add to a text view to support extended text gestures.

protocol BETextInteractionDelegate

A set of methods that informs you about selection changes in text views.

protocol BEResponderEditActions

A set of methods that defines extended interactions in browser text views.

enum BEGestureType

protocol BEResponderEditActions

A set of methods that defines extended interactions in browser text views.

### Text selection

protocol BETextSelectionDirectionNavigation

struct BESelectionFlags

enum BESelectionTouchPhase

### Keyboard input

class BEKeyEntry

A class that represents a keyboard event in the text system.

class BEKeyEntryContext

A class that describes a key event and the text document with which the event is associated.

enum BEKeyModifierFlags

An enumeration that records the state of the shift-modifier keys.

### Replacements and AutoFill

class BEAutoFillTextSuggestion

class BETextAlternatives

class BETextDocumentContext

Information about the text surrounding a selection in a document.

class BETextDocumentRequest

struct Options

class BETextSuggestion

A text suggestion to insert into a document.

struct BETextReplacementOptions

### Information about text

protocol BEExtendedTextInputTraits

struct BEDirectionalTextRange

## See Also

### Web content

View coordination

Display content in the browser’s UI that an extension renders.

class BEWebAppManifest

An object that represents a web app manifest.

