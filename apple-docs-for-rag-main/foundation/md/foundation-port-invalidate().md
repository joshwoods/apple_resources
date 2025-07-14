

- Foundation
- Port
-  invalidate() 

Instance Method

# invalidate()

Marks the receiver as invalid and posts an didBecomeInvalidNotification to the default notification center.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func invalidate()
```

## Discussion

You must call this method before releasing a port object (or removing strong references to it if your application is garbage collected).

## See Also

### Validation

var isValid: Bool

A Boolean value that indicates whether the receiver is valid.

