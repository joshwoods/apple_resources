

- Foundation
- NSEnumerationOptions
-  reverse 

Type Property

# reverse

Specifies that the enumeration should be performed in reverse.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var reverse: NSEnumerationOptions { get }
```

## Discussion

This option is available for `NSArray` and `NSIndexSet` classes; its behavior is undefined for `NSDictionary` and `NSSet` classes, or when combined with the `NSEnumerationConcurrent` flag.

## See Also

### Constants

static var concurrent: NSEnumerationOptions

Specifies that the Block enumeration should be concurrent.

