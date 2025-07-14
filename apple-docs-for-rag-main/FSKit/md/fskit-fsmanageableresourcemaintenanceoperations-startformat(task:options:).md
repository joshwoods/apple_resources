

- FSKit
- FSManageableResourceMaintenanceOperations
-  startFormat(task:options:) 

Instance Method

# startFormat(task:options:)

Starts formatting the file system with the given options.

macOS 15.4+

``` source
func startFormat(
    task: FSTask,
    options: FSTaskOptions
) throws -> Progress
```

**Required**

## Parameters 

`task`  

A task object you use to communicate back to the client.

`options`  

Options for performing the format.

## Return Value

An NSProgress object that you use to update progress as the format operation progresses. Return `nil` if starting to format the file system encountered an error.

