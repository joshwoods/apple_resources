

- Foundation
- NSKeyValueObservingOptions
-  old 

Type Property

# old

Indicates that the change dictionary should contain the old attribute value, if applicable.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var old: NSKeyValueObservingOptions { get }
```

## See Also

### Constants

static var new: NSKeyValueObservingOptions

Indicates that the change dictionary should provide the new attribute value, if applicable.

static var initial: NSKeyValueObservingOptions

If specified, a notification should be sent to the observer immediately, before the observer registration method even returns.

static var prior: NSKeyValueObservingOptions

Whether separate notifications should be sent to the observer before and after each change, instead of a single notification after the change.

