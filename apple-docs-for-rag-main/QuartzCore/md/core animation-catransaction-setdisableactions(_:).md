

- Core Animation
- CATransaction
-  setDisableActions(\_:) 

Type Method

# setDisableActions(\_:)

Sets whether actions triggered as a result of property changes made within this transaction group are suppressed.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
class func setDisableActions(_ flag: Bool)
```

## Parameters 

`flag`  

true, if actions should be disabled.

## Discussion

This is a convenience method that invokes setValue(_:forKey:) with an `NSNumber` containing a true for the kCATransactionDisableActions key.

## See Also

### Temporarily Disabling Property Animations

class func disableActions() -> Bool

Returns whether actions triggered as a result of property changes made within this transaction group are suppressed.

