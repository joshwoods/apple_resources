

- XPC
-  XPC_ACTIVITY_PRIORITY_UTILITY 

Global Variable

# XPC_ACTIVITY_PRIORITY_UTILITY

A string that indicates an activity is utility priority.

macOS 10.9+

``` source
let XPC_ACTIVITY_PRIORITY_UTILITY: UnsafePointer
```

## Discussion

Utility priority is intended for user-visible tasks such as fetching data from the network, copying files, or importing data.

## See Also

### Priority

let XPC_ACTIVITY_PRIORITY: UnsafePointer&lt;CChar>

A string property that indicates the priority of the activity.

let XPC_ACTIVITY_PRIORITY_MAINTENANCE: UnsafePointer&lt;CChar>

A string that indicates an activity is maintenance priority.

