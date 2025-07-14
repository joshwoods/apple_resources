

- UIKit
-  UIInputViewController 

Class

# UIInputViewController

The primary view controller for a custom keyboard app extension.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIInputViewController
```

## Mentioned in 

Handling text interactions in custom keyboards

Configuring open access for a custom keyboard

## Overview

To create a custom keyboard, first subclass the UIInputViewController class, then add your keyboard’s user interface to the inputView property of your subclass. In Xcode, you can start a custom keyboard by choosing the Custom Keyboard target template.

A custom keyboard can respond to user input events in the following ways:

- Add text in the form of an unattributed NSString object at the insertion point in the current text input object, by calling the insertText(_:) method on the textDocumentProxy property. This property provides that method through its conformance to the UIKeyInput protocol

- Delete text in a backward direction, starting at the insertion point, by calling the deleteBackward() method on the textDocumentProxy property.

- Switch to another keyboard in the set of user-enabled keyboards, by calling the advanceToNextInputMode() method.

- Dismiss the keyboard, by calling the dismissKeyboard() method.

Obtain textual context around the insertion point by reading the textDocumentProxy properties documentContextBeforeInput and documentContextAfterInput. To find out if the current text input object is empty, call the hasText method on the textDocumentProxy property. You can employ this textual context by considering it along with user input, to offer context-sensitive output to a document from your keyboard.

An input view controller conforms to the UITextInputDelegate protocol, allowing you to respond to changes in document content and position of the insertion point.

To present an appropriate keyboard layout, respond to the current text input object’s UIKeyboardType property. For each keyboard type trait you support, change the contents of your primary view accordingly.

For more about creating a custom keyboard, read Custom Keyboard in App Extension Programming Guide.

## Topics

### Providing a user interface for a custom keyboard

var inputView: UIInputView?

The primary view for the input view controller.

### Controlling a custom keyboard

func advanceToNextInputMode()

Switches to the next keyboard in the list of user-enabled keyboards.

func dismissKeyboard()

Dismisses the custom keyboard from the screen.

func handleInputModeList(from: UIView, with: UIEvent)

Supports interaction with the list of user-enabled keyboards.

### Interacting with a text input object

var textDocumentProxy: any UITextDocumentProxy

A proxy to the text input object that the custom keyboard is interacting with.

protocol UITextDocumentProxy

An object that provides textual context to a custom keyboard.

### Obtaining a supplementary lexicon

func requestSupplementaryLexicon(completion: (UILexicon) -> Void)

Obtains a supplementary lexicon of term pairs in a custom keyboard.

### Changing the primary language of a custom keyboard

var primaryLanguage: String?

The primary language for a custom keyboard.

### Configuring the keyboard behaviors

var needsInputModeSwitchKey: Bool

A Boolean value that indicates whether the keyboard must display an input switcher key.

var hasFullAccess: Bool

A Boolean value that indicates whether the keyboard has full access.

var hasDictationKey: Bool

A Boolean value that indicates whether the keyboard has a dictation key.

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITextInputDelegate
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Custom keyboard

protocol UITextDocumentProxy

An object that provides textual context to a custom keyboard.

protocol UIInputViewAudioFeedback

A property that enables a custom input or keyboard accessory view to play standard keyboard input clicks.

class UILexicon

A read-only array of term pairs, each in a lexicon entry object, for a custom keyboard.

class UILexiconEntry

A read-only term pair, available within a lexicon object, for a custom keyboard.

