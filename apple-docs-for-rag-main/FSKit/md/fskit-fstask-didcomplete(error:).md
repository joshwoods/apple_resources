

- FSKit
- FSTask
-  didComplete(error:) 

Instance Method

# didComplete(error:)

Informs the client that the task completed.

macOS 15.4+

``` source
func didComplete(error: (any Error)?)
```

## Parameters 

`error`  

`nil` if the task completed successfully; otherwise, an error that caused the task to fail.

