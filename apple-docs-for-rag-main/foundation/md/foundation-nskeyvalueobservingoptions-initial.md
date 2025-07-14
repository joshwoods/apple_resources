

- Foundation
- NSKeyValueObservingOptions
-  initial 

Type Property

# initial

If specified, a notification should be sent to the observer immediately, before the observer registration method even returns.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var initial: NSKeyValueObservingOptions { get }
```

## Discussion

The change dictionary in the notification will always contain an newKey entry if new is also specified but will never contain an oldKey entry. (In an initial notification the current value of the observed property may be old, but it’s new to the observer.) You can use this option instead of explicitly invoking, at the same time, code that is also invoked by the observer’s observeValue(forKeyPath:of:change:context:) method. When this option is used withaddObserver(_:forKeyPath:options:context:) a notification will be sent for each indexed object to which the observer is being added.

## See Also

### Constants

static var new: NSKeyValueObservingOptions

Indicates that the change dictionary should provide the new attribute value, if applicable.

static var old: NSKeyValueObservingOptions

Indicates that the change dictionary should contain the old attribute value, if applicable.

static var prior: NSKeyValueObservingOptions

Whether separate notifications should be sent to the observer before and after each change, instead of a single notification after the change.

