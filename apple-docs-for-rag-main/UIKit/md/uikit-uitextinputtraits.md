

- UIKit
-  UITextInputTraits 

Protocol

# UITextInputTraits

A set of methods that defines features for keyboard input to a text object.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UITextInputTraits : NSObjectProtocol
```

## Mentioned in 

Configuring a custom keyboard interface

## Overview

For a custom text object to support keyboard input, it must adopt this protocol to interact properly with the text-input management system. The UITextField and UITextView classes automatically support this protocol.

## Topics

### Configuring the keyboard appearance

var keyboardType: UIKeyboardType

The keyboard type for the text object.

enum UIKeyboardType

Constants that specify the type of keyboard to display for a text-based view.

var keyboardAppearance: UIKeyboardAppearance

The appearance style of the keyboard for the text object.

enum UIKeyboardAppearance

Constants that specify the appearance of the keyboard for a text-based view.

var returnKeyType: UIReturnKeyType

The visible title of the Return key.

enum UIReturnKeyType

Constants that specify the text string that displays in the Return key of a keyboard.

var textContentType: UITextContentType!

The semantic meaning for a text input area.

struct UITextContentType

Constants that identify the semantic meaning for a text-entry area.

### Managing the keyboard behavior

var isSecureTextEntry: Bool

A Boolean value that indicates whether a text object disables copying, and in some cases, prevents recording/broadcasting and also hides the text.

var enablesReturnKeyAutomatically: Bool

A Boolean value that indicates whether the system automatically enables the Return key when the user enters text.

### Managing spelling and autocorrection

var autocapitalizationType: UITextAutocapitalizationType

The autocapitalization style for the text object.

enum UITextAutocapitalizationType

The autocapitalization behavior of a text-based view.

var autocorrectionType: UITextAutocorrectionType

The autocorrection style for the text object.

enum UITextAutocorrectionType

The autocorrection behavior of a text-based view.

var spellCheckingType: UITextSpellCheckingType

The spell-checking style for the text object.

enum UITextSpellCheckingType

The spell-checking behavior of a text-based view.

var inlinePredictionType: UITextInlinePredictionType

The behavior of inline text predictions for a text-entry area.

enum UITextInlinePredictionType

Constants that identify the behavior of inline text predictions for a text-entry area.

### Configuring the autoformatting behaviors

var smartQuotesType: UITextSmartQuotesType

The configuration state for smart quotes.

enum UITextSmartQuotesType

Constants that indicate whether to enable or disable smart quotes.

var smartDashesType: UITextSmartDashesType

The configuration state for smart dashes.

enum UITextSmartDashesType

Constants that specify the automatic conversion behavior between hyphens and en or em dashes.

var smartInsertDeleteType: UITextSmartInsertDeleteType

The configuration state for the smart insertion and deletion of space characters.

enum UITextSmartInsertDeleteType

Constants that specify whether to automatically insert extra spaces after a paste operation or to delete them after a cut or delete operation.

### Configuring the writing tools experience

var writingToolsBehavior: UIWritingToolsBehavior

The writing tools experience to support in the current view.

enum UIWritingToolsBehavior

Constants that specify the writing tools experience for the underlying view.

### Configuring Smart Replies

var conversationContext: UIConversationContext?

A reference to a conversation, such as a mail or messaging thread.

### Configuring Password AutoFill

Password AutoFill

Streamline your app’s login and onboarding procedures.

class UITextInputPasswordRules

A class that represents password rules for a text input field.

### Configuring math expression completion

var mathExpressionCompletionType: UITextMathExpressionCompletionType

enum UITextMathExpressionCompletionType

### Instance Properties

var allowedWritingToolsResultOptions: UIWritingToolsResultOptions

var passwordRules: UITextInputPasswordRules?

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- UIKeyInput
- UITextDocumentProxy
- UITextDraggable
- UITextDroppable
- UITextInput

### Conforming Types

- UISearchBar
- UISearchTextField
- UITextField
- UITextView

## See Also

### Text input

protocol UITextInput

A set of methods for interacting with the text input system and enabling features in documents.

protocol UITextInputDelegate

An intermediary between a document and the text input system.

protocol UIKeyInput

A set of methods a responder uses to implement simple text entry.

class UITextInputContext

An object that reports the type of input your app receives.

class UITextInputMode

The current text input mode.

class UITextInputAssistantItem

An object that manages custom bar button items that you add to the shortcuts bar above the keyboard on iPad.

class UIDictationPhrase

An object that represents the textual interpretation of a spoken phrase that the user dictates.

