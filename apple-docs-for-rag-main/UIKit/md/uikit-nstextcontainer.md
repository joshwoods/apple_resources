

- UIKit
-  NSTextContainer 

Class

# NSTextContainer

A region where text layout occurs.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
class NSTextContainer
```

## Overview

An NSLayoutManager uses NSTextContainer to determine where to break lines, lay out portions of text, and so on. An NSTextContainer object typically defines rectangular regions, but you can define exclusion paths inside the text container to create regions where text doesn’t flow. You can also subclass to create text containers with nonrectangular regions, such as circular regions, regions with holes in them, or regions that flow alongside graphics.

You can access instances of the NSTextContainer, NSLayoutManager, and NSTextStorage classes from threads other than the main thread as long as the app guarantees access from only one thread at a time.

## Topics

### Creating a text container

init(size: CGSize)

Initializes a text container with a specified bounding rectangle.

init(coder: NSCoder)

Creates a text container from data in an unarchiver.

### Managing text components

var layoutManager: NSLayoutManager?

The text container’s layout manager.

var textLayoutManager: NSTextLayoutManager?

func replaceLayoutManager(NSLayoutManager)

Replaces the layout manager for the group of text system objects that contains the text container.

weak var textView: NSTextView? { get set }

The text container’s text view.

### Defining the container shape

var size: CGSize

The size of the text container’s bounding rectangle.

var exclusionPaths: [UIBezierPath]

An array of path objects that represents the regions where text doesn’t display in the text container.

var lineBreakMode: NSLineBreakMode

The behavior of the last line inside the text container.

var widthTracksTextView: Bool

A Boolean that controls whether the text container adjusts the width of its bounding rectangle when its text view resizes.

var heightTracksTextView: Bool

A Boolean that controls whether the text container adjusts the height of its bounding rectangle when its text view resizes.

### Constraining text layout

var maximumNumberOfLines: Int

The maximum number of lines that the text container can store.

var lineFragmentPadding: CGFloat

The value for the text inset within line fragment rectangles.

func lineFragmentRect(forProposedRect: CGRect, at: Int, writingDirection: NSWritingDirection, remaining: UnsafeMutablePointer&lt;CGRect>?) -> CGRect

Returns the bounds of a line fragment rectangle inside the text container for the proposed rectangle.

var isSimpleRectangularTextContainer: Bool

A Boolean that indicates whether the text container’s region is a rectangle with no holes or gaps, and whose edges are parallel to the text view’s coordinate system axes.

### Deprecated

convenience init(containerSize aContainerSize: NSSize)

Initializes a text container with a specified bounding rectangle.

func lineFragmentRect(forProposedRect proposedRect: NSRect, sweepDirection: NSLineSweepDirection, movementDirection: NSLineMovementDirection, remaining remainingRect: NSRectPointer?) -> NSRect

Calculates and returns the longest rectangle available in the proposed rectangle for displaying text.

func contains(_ point: NSPoint) -> Bool

Queries whether a point lies within the text container’s region or on the region’s edge—not simply within its bounding rectangle.

Deprecated

var containerSize: NSSize { get set }

The size of the text container’s bounding rectangle.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- NSTextLayoutOrientationProvider

## See Also

### Layout

Using TextKit 2 to interact with text

Interact with text by managing text selection and inserting custom text elements.

Display text with a custom layout

Lay out text in a custom-shaped container and apply glyph substitutions.

class NSTextLayoutManager

The primary class that you use to manage text layout and presentation for custom text displays.

class NSTextLayoutFragment

A class that represents the layout fragment typically corresponding to a rendering surface, such as a layer or view subclass.

class NSTextLineFragment

A class that represents a line fragment as a single textual layout and rendering unit inside a text layout fragment.

class NSTextViewportLayoutController

Manages the layout process inside the viewport interacting with its delegate.

protocol NSTextLayoutOrientationProvider

A set of methods that define the orientation of text for an object.

