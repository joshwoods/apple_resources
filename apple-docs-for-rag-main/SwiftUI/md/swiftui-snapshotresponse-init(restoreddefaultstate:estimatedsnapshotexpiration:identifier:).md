

- SwiftUI
- SnapshotResponse
-  init(restoredDefaultState:estimatedSnapshotExpiration:identifier:) 

Initializer

# init(restoredDefaultState:estimatedSnapshotExpiration:identifier:)

Creates a snapshot response.

watchOS 9.0+

``` source
init(
    restoredDefaultState: Bool = false,
    estimatedSnapshotExpiration: Date? = nil,
    identifier: String? = nil
)
```

## Parameters 

`restoredDefaultState`  

Pass `true` if your app has navigated back to its default launch scene.

`estimatedSnapshotExpiration`  

The preferred date and time for the next background snapshot refresh task. Use distantFuture if you don’t want to schedule the next refresh.

`identifier`  

A custom string to associate with the next background snapshot refresh task. This value is assigned to the next snapshot task’s `TaskData` userInfo property. Pass `nil` if you don’t want to associate any identifier with the next task.

