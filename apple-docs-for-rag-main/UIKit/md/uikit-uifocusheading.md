

- UIKit
-  UIFocusHeading 

Structure

# UIFocusHeading

The general type of an event.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
struct UIFocusHeading
```

## Overview

You obtain the direction of the focus from the focusHeading property.

## Topics

### Constants

static var up: UIFocusHeading

The focus update is heading in the up direction.

static var down: UIFocusHeading

The focus update is heading in the down direction.

static var left: UIFocusHeading

The focus update is heading in the left direction.

static var right: UIFocusHeading

The focus update is heading in the right direction.

static var next: UIFocusHeading

The focus update is heading to the next item.

static var previous: UIFocusHeading

The focus update is heading to the previous item.

static var first: UIFocusHeading

The focus update is heading to the first item.

static var last: UIFocusHeading

The focus update is heading to the last item.

### Initializers

init(rawValue: UInt)

Creates a focus heading structure with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Locating focus direction

var previouslyFocusedView: UIView?

The view that was focused before the focus update.

var nextFocusedView: UIView?

The view that takes the focus after the focus update.

var focusHeading: UIFocusHeading

The heading in which the focus update is occurring.

