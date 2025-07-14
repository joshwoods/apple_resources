

- InputMethodKit
-  IMKInputController 

Class

# IMKInputController

The `IMKInputController` class provides a base class for custom input controller classes. The IMKServer class, which is allocated in the main function of an input method, creates an input controller object for each input session created by a client application. For every input session there is a corresponding `IMKInputController` object.

macOS 10.5+

``` source
class IMKInputController
```

## Overview

An `IMKInputController` object controls text input on the input method side. It manages events and text from the applications and converted text from the input method engine. `IMKInputController` implements fully the IMKStateSetting and IMKMouseHandling protocols. Typically you do not need to override this class, but you do need to provide a delegate object that implements the methods that your are interested in. The `IMKInputController` versions of the protocol methods check whether the delegate object implements a method, and calls the delegate version if it exists.

## Topics

### Initializing an Input Controller

init!(server: IMKServer!, delegate: Any!, client: Any!)

Initializes the input control by setting the delegate.

### Working with Ranges

func compositionAttributes(at: NSRange) -> NSMutableDictionary!

Returns a dictionary of text attributes.

func selectionRange() -> NSRange

Returns where the range of the selection that should be placed inside marked text.

func replacementRange() -> NSRange

Returns the range in the client document that the text should replace.

func mark(forStyle: Int, at: NSRange) -> [AnyHashable : Any]!

Returns a dictionary of text attributes that can mark a range of an attributed string to send to a client.

### Managing the Delegate

func delegate() -> Any!

Returns the delegate for input controller object.

func setDelegate(Any!)

Sets the delegate for input controller object.

### Getting the Client and Server Objects

func server() -> IMKServer!

Returns the server object that manages the input controller.

func client() -> (any IMKTextInput &amp; NSObjectProtocol)!

Returns the client object associated with the input controller.

### Tracking Selections

func annotationSelected(NSAttributedString!, forCandidate: NSAttributedString!)

Sends the selected candidate string and annotation string to the input controller.

func candidateSelectionChanged(NSAttributedString!)

Informs an input controller that the current candidate selection in the candidate window has changed.

func candidateSelected(NSAttributedString!)

Informs an input controller that a new candidate is selected.

### Managing Composition

func updateComposition()

Informs the input controller that the composition has changed.

func cancelComposition()

Stops the current composition and replaces marked text with the original text.

### Hiding the User Interface

func hidePalettes()

Informs an input method that it should close any visible user interface.

### Working with Custom Commands

func doCommand(by: Selector!, command: [AnyHashable : Any]!)

Passes commands that are not generated as part of the text input process.

func menu() -> NSMenu!

Returns a menu of commands that are specific to an input method.

### Instance Methods

func inputControllerWillClose()

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- IMKMouseHandling
- IMKStateSetting
- NSObjectProtocol

## See Also

### Classes

class IMKCandidates

The `IMKCandidates` class presents candidates to users and notifies the appropriate IMKInputController object when the user selects a candidate. **Candidates** are alternate characters for a given input sequence. The `IMKCandidates` class supports using a candidates window in your input method; using `IMKCandidates` is optional. Not all input methods require them.

class IMKServer

The `IMKServer` class manages client connections to your input method. When you write the main function for your input method, you create an `IMKServer` object. You should never need to override this class.

