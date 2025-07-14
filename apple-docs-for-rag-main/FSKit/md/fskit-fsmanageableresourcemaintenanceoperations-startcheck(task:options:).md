

- FSKit
- FSManageableResourceMaintenanceOperations
-  startCheck(task:options:) 

Instance Method

# startCheck(task:options:)

Starts checking the file system with the given options.

macOS 15.4+

``` source
func startCheck(
    task: FSTask,
    options: FSTaskOptions
) throws -> Progress
```

**Required**

## Parameters 

`task`  

A task object you use to communicate back to the client.

`options`  

Options for performing the check.

## Return Value

An NSProgress object that you use to update progress as the check operation progresses. Return `nil` if starting the file system check encountered an error.

