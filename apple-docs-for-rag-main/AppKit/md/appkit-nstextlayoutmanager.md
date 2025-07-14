

- AppKit
-  NSTextLayoutManager 

Class

# NSTextLayoutManager

The primary class that you use to manage text layout and presentation for custom text displays.

macOS 12.0+

``` source
class NSTextLayoutManager
```

## Overview

`NSTextLayoutManager` is the centerpiece of the TextKit object network that maintains the layout geometry through an array of NSTextContainer objects. It lays out results using NSTextLayoutFragment and NSTextElement objects vended from a NSTextContentManager that participates in the content layout process.

## Topics

### Creating a layout manager

init()

Creates a new text layout manager.

init?(coder: NSCoder)

Creates a new text layout manager with the coder you provide.

### Configuring global layout manager options

var layoutQueue: OperationQueue?

The queue that the framework dispatches layout operations on.

var renderingAttributesValidator: ((NSTextLayoutManager, NSTextLayoutFragment) -> Void)?

A callback block that the framework invokes whenever the text layout manager needs to validate the rendering attributes for the range.

var usesFontLeading: Bool

A Boolean value that controls whether the framework uses the leading information specified by the font when laying out text.

var usesHyphenation: Bool

A Boolean values that controls whether the text layout manager attempts to hyphenate when wrapping lines.

var limitsLayoutForSuspiciousContents: Bool

A Boolean value that controls internal security analysis for malicious inputs and activates defensive behaviors.

### Managing the layout process

var delegate: (any NSTextLayoutManagerDelegate)?

The delegate for the text layout manager object.

protocol NSTextLayoutManagerDelegate

Optional methods that delegates implement to respond to layout changes.

### Accessing the text storage

var textContentManager: NSTextContentManager?

Returns the text content manager associated with this text layout manager.

var textContainer: NSTextContainer?

The text container object that provides geometric information for the layout destination.

var textSelectionNavigation: NSTextSelectionNavigation

Returns a text selection manager configured to have the text layout manager as its data source.

var textSelections: [NSTextSelection]

An array of text selections associated by the text layout manager.

var usageBoundsForTextContainer: CGRect

Returns the usage bounds for the text container.

func enumerateTextSegments(in: NSTextRange, type: NSTextLayoutManager.SegmentType, options: NSTextLayoutManager.SegmentOptions, using: (NSTextRange?, CGRect, CGFloat, NSTextContainer) -> Bool)

Enumerates text segments of a specific type and in the text range you provide.

func replace(NSTextContentManager)

Replaces the current text content manager with a new one you provide.

func replaceContents(in: NSTextRange, with: NSAttributedString)

Replaces content at the location you specify with an attributed string you provide.

func replaceContents(in: NSTextRange, with: [NSTextElement])

Replaces content at the location you specify with the text elements string you provide.

### Adjusting rendering

class var linkRenderingAttributes: [NSAttributedString.Key : Any]

Returns the default set of attributes for rendering a link.

func addRenderingAttribute(NSAttributedString.Key, value: Any?, for: NSTextRange)

Sets the rendering attribute for the value and range you specify.

func enumerateRenderingAttributes(from: any NSTextLocation, reverse: Bool, using: (NSTextLayoutManager, [NSAttributedString.Key : Any], NSTextRange) -> Bool)

Enumerates the rendering attributes from a location you specify.

func renderingAttributes(forLink: Any, at: any NSTextLocation) -> [NSAttributedString.Key : Any]

Returns a dictionary of rendering attributes for rendering a link.

func invalidateRenderingAttributes(for: NSTextRange)

Invalidates the rendering attributes of the specified text range.

func removeRenderingAttribute(NSAttributedString.Key, for: NSTextRange)

Removes the rendering attribute from the specified text range.

func setRenderingAttributes([NSAttributedString.Key : Any], for: NSTextRange)

Sets the rendering attributes for the range you specify.

### Causing layout generation

var textViewportLayoutController: NSTextViewportLayoutController

Returns text viewport layout controller associated with the layout manager’s text container.

func invalidateLayout(for: NSTextRange)

Invalidates the layout information for specified text range.

func textLayoutFragment(for: any NSTextLocation) -> NSTextLayoutFragment?

Returns the text layout fragment from the document at the specified location.

func textLayoutFragment(for: CGPoint) -> NSTextLayoutFragment?

Returns the text layout fragment at the position you specify in the text container.

func ensureLayout(for: CGRect)

Performs the layout for filling the bounds you specify inside the last text container.

func ensureLayout(for: NSTextRange)

Performs the layout for specified text range.

func enumerateTextLayoutFragments(from: (any NSTextLocation)?, options: NSTextLayoutFragment.EnumerationOptions, using: (NSTextLayoutFragment) -> Bool) -> (any NSTextLocation)?

Enumerates the text layout fragments starting at the specified location.

enum SegmentType

Values that describe the rendering of selection boundaries.

struct SegmentOptions

Values that describe where and how the framework extends segments of a selection.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- NSTextSelectionDataSource

## See Also

### Layout

Using TextKit 2 to interact with text

Interact with text by managing text selection and inserting custom text elements.

class NSTextContainer

A region where text layout occurs.

class NSTextLayoutFragment

A class that represents the layout fragment typically corresponding to a rendering surface, such as a layer or view subclass.

class NSTextLineFragment

A class that represents a line fragment as a single textual layout and rendering unit inside a text layout fragment.

class NSTextViewportLayoutController

Manages the layout process inside the viewport interacting with its delegate.

protocol NSTextLayoutOrientationProvider

A set of methods that define the orientation of text for an object.

