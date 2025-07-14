

- Foundation
- NSBackgroundActivityScheduler
-  init(identifier:) 

Initializer

# init(identifier:)

Initializes a background activity scheduler object with a specified unique identifier.

macOS 10.10+

``` source
init(identifier: String)
```

## Parameters 

`identifier`  

A unique string, in reverse DNS notation, that identifies the activity. For example, `com.example.MyApp.updatecheck`. `nil` and zero-length strings are not allowed.

## Return Value

A new background activity scheduler object of type NSBackgroundActivityScheduler.

## Discussion

The string passed to the `identifier` parameter should remain constant for an activity across launches of your app because the system uses this unique identifier to track the number of times the activity has run and to improve the heuristics for deciding when to run it again in the future. See Create a Scheduler.

## See Also

### Related Documentation

var identifier: String

A unique reverse DNS notation string, such as `com.example.MyApp.updatecheck`, that identifies the activity.

