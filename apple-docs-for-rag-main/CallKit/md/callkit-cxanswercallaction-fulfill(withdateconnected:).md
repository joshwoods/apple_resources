

- CallKit
- CXAnswerCallAction
-  fulfill(withDateConnected:) 

Instance Method

# fulfill(withDateConnected:)

Reports the successful execution of the action at the specified time.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
func fulfill(withDateConnected dateConnected: Date)
```

## Parameters 

`dateConnected`  

The time that the call was connected. A call is considered connected when both caller and callee can start communicating.

## Discussion

Use this method instead of fulfill() to note a time other than the current time that the call connected.

