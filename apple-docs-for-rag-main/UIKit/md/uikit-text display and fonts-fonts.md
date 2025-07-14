

- UIKit
-  Text display and fonts 

API Collection

# Text display and fonts

Display text, manage fonts, and check spelling.

## Topics

### Text views

class UILabel

A view that displays one or more lines of informational text.

class UITextField

An object that displays an editable text area in your interface.

class UITextView

A scrollable, multiline text region.

Drag and drop customization

Extend the standard drag and drop support for text views to include custom types of content.

### Text bounds sizing

protocol UILetterformAwareAdjusting

The typographic bounds-sizing behavior to handle text with fonts that contain oversize characters.

### Text formatting

class UITextFormattingCoordinator

An object that coordinates text formatting using the standard Mac font panel.

typealias UITextAttributesConversionHandler

A handler for updating text with current font panel settings.

### Fonts

Scaling Fonts Automatically

Scale text in your interface automatically using Dynamic Type.

Adding a Custom Font to Your App

Add a custom font to your app and use it in your app’s interface.

class UIFont

An object that provides access to the font’s characteristics.

class UIFontDescriptor

A collection of attributes that describes a font.

struct SymbolicTraits

Constants that describe the stylistic aspects of a font.

class UIFontMetrics

A utility object for obtaining custom fonts that scale to support Dynamic Type.

### Font picker

class UIFontPickerViewController

A view controller that manages the interface for selecting a font that the system provides or the user installs.

protocol UIFontPickerViewControllerDelegate

A set of optional methods for receiving messages about the user’s interaction with the font picker.

class Configuration

The filters and display settings a font picker view controller uses to set up a font picker.

### Spell checking

class UITextChecker

An object to check a string (usually the text of a document) for misspelled words.

### Text manipulations

init(_ nsTextAlignment: NSTextAlignment)

Converts a UIKit text alignment constant value to the matching constant value that Core Text uses.

init(CTTextAlignment)

Converts a Core Text alignment constant value to the matching constant value in UIKit.

### Metrics

class UITextPosition

A position in a text container—that is, an index into the backing string in a text-display view.

class UITextRange

A range of characters in a text container with a starting index and an ending index in string backing a text-entry object.

class UITextSelectionRect

An encapsulation of information about a selected range of text in a document.

## See Also

### Text

TextKit

Manage text storage and perform custom layout of text-based content in your app’s views.

Keyboards and input

Configure the system keyboard, create your own keyboards to handle input, or detect key presses on a physical keyboard.

Writing Tools

Add support for Writing Tools to your app’s text views.

Handwriting recognition

Configure text fields and custom views that accept text to handle input from Apple Pencil.

