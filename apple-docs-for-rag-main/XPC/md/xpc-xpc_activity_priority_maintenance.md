

- XPC
-  XPC_ACTIVITY_PRIORITY_MAINTENANCE 

Global Variable

# XPC_ACTIVITY_PRIORITY_MAINTENANCE

A string that indicates an activity is maintenance priority.

macOS 10.9+

``` source
let XPC_ACTIVITY_PRIORITY_MAINTENANCE: UnsafePointer
```

## Discussion

Maintenance priority is intended for user-invisible maintenance tasks such as garbage collection or optimization.

## See Also

### Priority

let XPC_ACTIVITY_PRIORITY: UnsafePointer&lt;CChar>

A string property that indicates the priority of the activity.

let XPC_ACTIVITY_PRIORITY_UTILITY: UnsafePointer&lt;CChar>

A string that indicates an activity is utility priority.

