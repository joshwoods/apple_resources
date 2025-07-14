

- UIKit
-  NSTextLayoutManagerDelegate 

Protocol

# NSTextLayoutManagerDelegate

Optional methods that delegates implement to respond to layout changes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
protocol NSTextLayoutManagerDelegate : NSObjectProtocol
```

## Topics

### Responding to layout changes

func textLayoutManager(NSTextLayoutManager, renderingAttributesForLink: Any, at: any NSTextLocation, defaultAttributes: [NSAttributedString.Key : Any]) -> [NSAttributedString.Key : Any]?

The method the framework calls to return a dictionary of attributes for rendering a link attribute name.

func textLayoutManager(NSTextLayoutManager, shouldBreakLineBefore: any NSTextLocation, hyphenating: Bool) -> Bool

The method the framework calls to determine the soft line break point.

func textLayoutManager(NSTextLayoutManager, textLayoutFragmentFor: any NSTextLocation, in: NSTextElement) -> NSTextLayoutFragment

The method the framework calls to give the delegate an opportunity to return a custom text layout fragment.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Managing the layout process

var delegate: (any NSTextLayoutManagerDelegate)?

The delegate for the text layout manager object.

