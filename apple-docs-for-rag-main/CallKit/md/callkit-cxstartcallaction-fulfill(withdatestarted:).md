

- CallKit
- CXStartCallAction
-  fulfill(withDateStarted:) 

Instance Method

# fulfill(withDateStarted:)

Reports the successful execution of the action at the specified time.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
func fulfill(withDateStarted dateStarted: Date)
```

## Parameters 

`dateStarted`  

The time that the call was started. A call is considered started when its invitation has been sent to the remote callee.

## Discussion

Use this method instead of fulfill() to note a time other than the current time that the call started.

