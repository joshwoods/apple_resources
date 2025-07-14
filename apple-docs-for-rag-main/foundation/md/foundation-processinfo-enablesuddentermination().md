

- Foundation
- ProcessInfo
-  enableSuddenTermination() 

Instance Method

# enableSuddenTermination()

Enables the application for quick killing using sudden termination.

macOS 10.6+

``` source
func enableSuddenTermination()
```

## Discussion

This method decrements the sudden termination counter. When the termination counter reaches `0` the application allows sudden termination.

By default the sudden termination counter is set to 1. This can be overridden in your application Info.plist. See Support Sudden Termination for more information and debugging suggestions.

## See Also

### Sudden Application Termination

func disableSuddenTermination()

Disables the application for quickly killing using sudden termination.

