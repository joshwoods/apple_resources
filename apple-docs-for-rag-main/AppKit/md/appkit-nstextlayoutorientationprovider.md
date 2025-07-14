

- AppKit
-  NSTextLayoutOrientationProvider 

Protocol

# NSTextLayoutOrientationProvider

A set of methods that define the orientation of text for an object.

macOS

``` source
protocol NSTextLayoutOrientationProvider
```

## Overview

In macOS, the NSTextContainer and NSTextView classes adopt this protocol; in iOS, only the NSTextContainer class implements it. An NSTextContainer object returns the value from its associated text view when present; otherwise, it returns NSLayoutManager.TextLayoutOrientation.horizontal by default. If you define a custom NSTextContainer object, you can override this method and return NSLayoutManager.TextLayoutOrientation.vertical to support laying out text vertically.

## Topics

### Getting layout orientation

var layoutOrientation: NSLayoutManager.TextLayoutOrientation

The default layout orientation.

**Required**

enum TextLayoutOrientation

Constants that describe the text layout orientation.

## Relationships

### Conforming Types

- NSTextContainer
- NSTextView

## See Also

### Layout

Using TextKit 2 to interact with text

Interact with text by managing text selection and inserting custom text elements.

class NSTextLayoutManager

The primary class that you use to manage text layout and presentation for custom text displays.

class NSTextContainer

A region where text layout occurs.

class NSTextLayoutFragment

A class that represents the layout fragment typically corresponding to a rendering surface, such as a layer or view subclass.

class NSTextLineFragment

A class that represents a line fragment as a single textual layout and rendering unit inside a text layout fragment.

class NSTextViewportLayoutController

Manages the layout process inside the viewport interacting with its delegate.

