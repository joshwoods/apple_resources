

- CallKit
- CXEndCallAction
-  fulfill(withDateEnded:) 

Instance Method

# fulfill(withDateEnded:)

Reports the successful execution of the action at the specified time.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
func fulfill(withDateEnded dateEnded: Date)
```

## Parameters 

`dateEnded`  

The time that the call was ended. A call is considered ended when the user disconnects or all other callers disconnect.

## Discussion

Use this method instead of fulfill() to note a time other than the current time that the call ended.

