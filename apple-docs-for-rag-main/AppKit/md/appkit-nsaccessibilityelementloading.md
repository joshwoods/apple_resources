

- AppKit
-  NSAccessibilityElementLoading 

Protocol

# NSAccessibilityElementLoading

A role-based protocol that declares the minimum interface necessary for an accessibility element to support loading.

macOS 10.13+

``` source
protocol NSAccessibilityElementLoading : NSObjectProtocol
```

## Overview

You can further enhance the adopting element by implementing any of the information properties or action methods that the NSAccessibilityProtocol protocol declares.

Note

Any class that adopts this protocol must implement all of its methods, and the required methods of any protocol it inherits from. The compiler may require you to override some methods that your ancestors have already implemented. Simply follow the compiler’s warnings, and reimplement these methods as necessary.

## Topics

### Supporting Accessibility

func accessibilityElement(withToken: NSAccessibilityLoadingToken) -> (any NSAccessibilityElementProtocol)?

Loads the target accessibility element with the specified load token.

**Required**

func accessibilityRangeInTargetElement(withToken: NSAccessibilityLoadingToken) -> NSRange

Returns the range that specifies the area of interest in text-based accessibility elements with the specified load token.

typealias NSAccessibilityLoadingToken

A token type for loading accessibility elements.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Loading

protocol NSAccessibilityProgressIndicator

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a progress indicator.

