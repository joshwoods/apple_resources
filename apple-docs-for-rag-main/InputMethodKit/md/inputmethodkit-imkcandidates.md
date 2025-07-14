

- InputMethodKit
-  IMKCandidates 

Class

# IMKCandidates

The `IMKCandidates` class presents candidates to users and notifies the appropriate IMKInputController object when the user selects a candidate. **Candidates** are alternate characters for a given input sequence. The `IMKCandidates` class supports using a candidates window in your input method; using `IMKCandidates` is optional. Not all input methods require them.

macOS 10.5+

``` source
@MainActor
class IMKCandidates
```

## Overview

When you create an `IMKCandidates` object, you attach it to the `IMKServer` object for your input method. You then need to override the `IMKInputController` methods `candidateSelectionChanged:` and `candidateSelected:` as well as implement a candidates method in your delegate object. The `IMKInputController` subclass supplies candidates to the `IMKCandidates` object by implementing the candidates method. When you are ready to display a candidates window, call the candidates method to update candidates and to show the candidates window.

## Topics

### Initializing a Candidates Window

init!(server: IMKServer!, panelType: IMKCandidatePanelType)

Returns the initialized `IMKCandidates` object.

### Managing Selection Keys

func setSelectionKeys([Any]!)

Sets the selection keys for the candidates.

func selectionKeys() -> [Any]!

Returns an array of `NSNumber` objects where each `NSNumber` object represents a virtual key code.

func setSelectionKeysKeylayout(TISInputSource!)

Sets the key layout that is used to map virtual key codes to characters.

func selectionKeysKeylayout() -> Unmanaged&lt;TISInputSource>!

Returns the key layout that maps virtual key codes to selection keys.

### Managing Window Visibility and Behavior

func show(IMKCandidatesLocationHint)

Shows the candidates window.

func hide()

Hides a candidates window, if it is visible.

func isVisible() -> Bool

Returns whether or not the candidates window is visible.

func setDismissesAutomatically(Bool)

Sets the state of the flag that determines whether the candidates window dismisses automatically.

func dismissesAutomatically() -> Bool

Returns the state of the flag that determines whether the candidates window dismisses automatically.

func update()

Updates the candidates that are displayed in the candidates window.

### Managing Window Type and Text Attributes

func panelType() -> IMKCandidatePanelType

Returns the style of the candidates window.

func setPanelType(IMKCandidatePanelType)

Sets the style of the candidates window.

func setAttributes([AnyHashable : Any]!)

Sets the style attributes for the candidates window.

func attributes() -> [AnyHashable : Any]!

Returns a dictionary of the style attributes used for the candidates window..

### Showing an Annotation Window

func showAnnotation(NSAttributedString!)

Displays an annotation string in an annotation window.

### Constants

typealias IMKCandidatePanelType

Types of candidates windows provide by the Input Method Kit.

typealias IMKCandidatesLocationHint

Hints that suggest where to place the candidates window.

IMKCandidatesOpacityAttributeName

The opacity level for a candidates window.

### Initializers

init!(server: IMKServer!, panelType: IMKCandidatePanelType, styleType: IMKStyleType)

### Instance Methods

func attachChild(IMKCandidates!, toCandidate: Int, type: IMKStyleType)

func candidateFrame() -> NSRect

func candidateIdentifier(atLineNumber: Int) -> Int

func candidateStringIdentifier(Any!) -> Int

func clearSelection()

func detachChild(Int)

func hideChild()

func lineNumberForCandidate(withIdentifier: Int) -> Int

func selectCandidate(Int)

func selectCandidate(withIdentifier: Int) -> Bool

func selectedCandidate() -> Int

func selectedCandidateString() -> NSAttributedString!

func setCandidateData([Any]!)

func setCandidateFrameTopLeft(NSPoint)

func show()

func showChild()

func showSublist([Any]!, subListDelegate: Any!)

## Relationships

### Inherits From

- NSResponder

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring

## See Also

### Classes

class IMKInputController

The `IMKInputController` class provides a base class for custom input controller classes. The IMKServer class, which is allocated in the main function of an input method, creates an input controller object for each input session created by a client application. For every input session there is a corresponding `IMKInputController` object.

class IMKServer

The `IMKServer` class manages client connections to your input method. When you write the main function for your input method, you create an `IMKServer` object. You should never need to override this class.

