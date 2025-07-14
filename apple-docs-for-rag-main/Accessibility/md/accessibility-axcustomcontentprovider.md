

- Accessibility
-  AXCustomContentProvider 

Protocol

# AXCustomContentProvider

The interface for customizing the accessibility content.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
protocol AXCustomContentProvider : NSObjectProtocol
```

## Topics

### Providing custom content

var accessibilityCustomContent: [AXCustomContent]!

An array of custom objects for creating accessible content.

**Required**

### Instance Properties

var accessibilityCustomContentBlock: AXCustomContentReturnBlock?

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Custom accessibility content

class AXCustomContent

Objects that define custom content and the timing of its output.

typealias AXCustomContentReturnBlock

