

- AppKit
-  NSTextFinderClient 

Protocol

# NSTextFinderClient

A set of methods implemented by objects that support searching using the NSTextFinder class and the in-window text find bar.

macOS

``` source
protocol NSTextFinderClient : NSObjectProtocol
```

## Overview

See NSTextFinder for details.

## Topics

### String Searching

var string: String

Allows the client to specify a single string for searching.

func string(at: Int, effectiveRange: NSRangePointer, endsWithSearchBoundary: UnsafeMutablePointer&lt;ObjCBool>) -> String

Returns the found string that is created by conceptually mapping its content to a single string, which is composed of a concatenation of all its substrings.

func stringLength() -> Int

Returns the full length of the conceptually concatenated string return by the `stringAtIndex:effectiveRange:endsWithSearchBoundary:` method.

### Replacing Text

func shouldReplaceCharacters(inRanges: [NSValue], with: [String]) -> Bool

Returns whether the specified strings should be replaced.

func replaceCharacters(in: NSRange, with: String)

Replaces the text in the specified range with the new string.

func didReplaceCharacters()

Specifies whether text characters were replaced.

### Selection Information

var isSelectable: Bool

Returns whether the text is selectable.

var allowsMultipleSelection: Bool

Returns whether multiple items can be selected.

var firstSelectedRange: NSRange

Returns the currently selected range.

var selectedRanges: [NSValue]

Returns an array of selected ranges.

### Text Edibility

var isEditable: Bool

Returns whether the text is editable.

### Determining and Displaying Text Locations

func contentView(at: Int, effectiveCharacterRange: NSRangePointer) -> NSView

Returns the view the context is displayed in.

func rects(forCharacterRange: NSRange) -> [NSValue]?

An array containing the located text in the content view’s coordinate system.

func scrollRangeToVisible(NSRange)

Scrolls the specified range such that it is visible.

var visibleCharacterRanges: [NSValue]

An array of visible character ranges.

### Drawing Glyphs

func drawCharacters(in: NSRange, forContentView: NSView)

Draw the glyphs for the requested character range as they are drawn in the given content view.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Search and Replace

class NSTextFinder

An optional search-and-replace find interface inside a view, usually a scroll view.

protocol NSTextFinderBarContainer

A protocol that provides a container in which the find bar is displayed.

