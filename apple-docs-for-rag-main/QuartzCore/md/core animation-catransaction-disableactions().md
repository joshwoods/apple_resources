

- Core Animation
- CATransaction
-  disableActions() 

Type Method

# disableActions()

Returns whether actions triggered as a result of property changes made within this transaction group are suppressed.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
class func disableActions() -> Bool
```

## Return Value

true if actions are disabled.

## Discussion

This is a convenience method that returns the `boolValue` for the value(forKey:) value returned by the kCATransactionDisableActions key.

## See Also

### Temporarily Disabling Property Animations

class func setDisableActions(Bool)

Sets whether actions triggered as a result of property changes made within this transaction group are suppressed.

