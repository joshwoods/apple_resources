

- AppKit
-  NSTextContentManager 

Class

# NSTextContentManager

An abstract class that defines the interface and a default implementation for managing the text document contents.

macOS 12.0+

``` source
class NSTextContentManager
```

## Mentioned in 

Adding Writing Tools support to a custom AppKit view

## Topics

### Creating a content manager

init()

Creates a new content manager.

init?(coder: NSCoder)

Creates a new content manager object from data in an unarchiver.

### Controlling backing store synchronization

var automaticallySynchronizesToBackingStore: Bool

Determines whether to automatically synchronize with the backing store when an editing transaction finishes.

### Performing transactions

var hasEditingTransaction: Bool

Indicates there’s an active editing transaction from the primary text layout manager.

func performEditingTransaction(() -> Void)

Performs an editing transaction and invokes a block upon completion.

func recordEditAction(in: NSTextRange, newTextRange: NSTextRange)

Records information about an edit action to the transaction.

### Working with layout managers

var primaryTextLayoutManager: NSTextLayoutManager?

The primary text layout manager for this content.

var textLayoutManagers: [NSTextLayoutManager]

The array of text layout managers associated with this text content manager.

var automaticallySynchronizesTextLayoutManagers: Bool

Determines if the framework should automatically synchronize all text layout managers when exiting an editing transaction.

func addTextLayoutManager(NSTextLayoutManager)

Adds the layout manager you provide to the list of layout managers.

func removeTextLayoutManager(NSTextLayoutManager)

Removes the layout manager you specifiy from the list of layout managers.

func synchronizeTextLayoutManagers((((any Error)?) -> Void)?)

Synchronizes changes to all nonprimary text layout managers.

### Customizing and validating text elements

var delegate: (any NSTextContentManagerDelegate)?

The delegate for the content manager object.

protocol NSTextContentManagerDelegate

The optional methods that delegates of content manager objects implement for customizing or validating text elements.

struct EnumerationOptions

Values that control the order in which the framework enumerates text elements.

### Finding a specific text element

func textElements(for: NSTextRange) -> [NSTextElement]

Returns an array of text elements that intersect with the range you specify.

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSTextContentStorage

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- NSTextElementProvider

## See Also

### Text management

class NSTextContentStorage

A concrete object for managing your view’s text content and generating the text elements necessary for layout.

class NSAttributedString

A string of text that manages data, layout, and stylistic information for ranges of characters to support rendering.

class NSMutableAttributedString

A mutable string with associated attributes (such as visual style, hyperlinks, or accessibility data) for portions of its text.

