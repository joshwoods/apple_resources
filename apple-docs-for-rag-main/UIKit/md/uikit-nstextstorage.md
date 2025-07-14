

- UIKit
-  NSTextStorage 

Class

# NSTextStorage

The fundamental storage mechanism of TextKit that contains the text managed by the system.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
class NSTextStorage
```

## Overview

NSTextStorage is a semi-concrete subclass of NSMutableAttributedString that adds behavior for managing a set of client NSLayoutManager objects. A text storage object notifies its layout managers of changes to its characters or attributes, which lets the layout managers redisplay the text as needed.

You can access a text storage object from any thread of your app, but your app must guarantee access from only one thread at a time.

In macOS, this class also defines properties for getting and setting scriptable attributes of NSTextStorage objects. Unless you’re dealing with scriptability, you shouldn’t access these properties directly. In particular, using the characters, words, or paragraphs properties is an inefficient way to manipulate the text storage, since accessing these properties involves the creation of many objects. Instead, use the text access methods defined by NSMutableAttributedString, NSAttributedString, NSMutableString, and NSString to perform character-level manipulation.

### Subclassing Notes

The NSTextStorage class implements change management through the beginEditing() and endEditing() methods, as well as verification of attributes, delegate handling, and layout management notification. The one aspect it doesn’t implement is managing the actual attributed string storage, which subclasses manage by overriding the two NSAttributedString primitives:

- string

- attributes(at:effectiveRange:)

Subclasses must also override two NSMutableAttributedString primitives:

- replaceCharacters(in:with:)

- setAttributes(_:range:)

These primitives should perform the change, then call edited(_:range:changeInLength:) to let the parent class know there are changes.

## Topics

### Processing the editing actions

var delegate: (any NSTextStorageDelegate)?

The delegate for the text storage object.

protocol NSTextStorageDelegate

The optional methods that delegates of text storage objects implement to handle text-edit processing.

### Accessing the layout managers

var layoutManagers: [NSLayoutManager]

The layout managers for the text storage object.

func addLayoutManager(NSLayoutManager)

Adds a layout manager to the text storage object’s set of layout managers.

func removeLayoutManager(NSLayoutManager)

Removes a layout manager from the text storage object’s set of layout managers.

### Managing edits

func edited(NSTextStorage.EditActions, range: NSRange, changeInLength: Int)

Tracks changes made to the text storage object, allowing the text storage to record the full extent of changes.

func processEditing()

Cleans up changes to the text storage object and notifies its delegate and layout managers of changes.

### Fixing the string attributes

func invalidateAttributes(in: NSRange)

Invalidates attributes in the specified range.

func ensureAttributesAreFixed(in: NSRange)

Ensures that attribute fixing occurs in the specified range.

var fixesAttributesLazily: Bool

A Boolean value that indicates whether the text storage object fixes attributes lazily.

### Determining the nature of changes

var editedMask: NSTextStorage.EditActions

A mask that describes the kinds of edits pending for the text storage object.

var editedRange: NSRange

The range of text that contains changes.

var changeInLength: Int

The difference between the current length of the edited range and its length before editing.

### Accessing scriptable properties

var attributeRuns: [NSTextStorage] { get set }

The text storage contents as an array of attribute runs.

var paragraphs: [NSTextStorage] { get set }

The text storage contents as an array of paragraphs.

var words: [NSTextStorage] { get set }

The text storage contents as an array of words.

var characters: [NSTextStorage] { get set }

The text storage contents as an array of characters.

var font: NSFont? { get set }

The font for the text storage.

var foregroundColor: NSColor? { get set }

The color for the text.

### Constants

struct EditActions

Constants that indicate the types of changes.

### Notifications

class let willProcessEditingNotification: NSNotification.Name

A notification that posts before a text storage begins processing edits.

class let didProcessEditingNotification: NSNotification.Name

A notification that posts after a text storage finishes processing edits.

### Accessing the storage controller

var textStorageObserver: (any NSTextStorageObserving)?

The observer for the text storage object.

protocol NSTextStorageObserving

Optional methods that delegates implement to handle editing and transaction processing.

## Relationships

### Inherits From

- NSMutableAttributedString

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSItemProviderReading
- NSItemProviderWriting
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### TextKit 1

class NSLayoutManager

An object that coordinates the layout and display of text characters.

