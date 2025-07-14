

- Security
-  SecTaskCreateFromSelf(\_:) 

Function

# SecTaskCreateFromSelf(\_:)

Creates a task object for the current task.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SecTaskCreateFromSelf(_ allocator: CFAllocator?) -> SecTask?
```

## Parameters 

`allocator`  

An allocator. Pass `NULL` to use the default.

## Return Value

A new task, or `NULL` on error. In Objective-C, call the CFRelease function to free this task’s memory when you are done with it.

