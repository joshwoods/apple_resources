

- CallKit
- CXCallObserverDelegate
-  callObserver(\_:callChanged:) 

Instance Method

# callObserver(\_:callChanged:)

Called when a call is changed.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
func callObserver(
    _ callObserver: CXCallObserver,
    callChanged call: CXCall
)
```

**Required**

## Parameters 

`callObserver`  

The call observer for the delegate.

`call`  

The call that has been changed.

