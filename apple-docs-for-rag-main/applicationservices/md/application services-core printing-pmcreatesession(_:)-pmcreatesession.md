

- Application Services
- Core Printing
-  PMCreateSession(\_:) 

Function

# PMCreateSession(\_:)

Creates and initializes a printing session object and creates a context for printing operations.

macOS 10.0+

``` source
func PMCreateSession(_ printSession: UnsafeMutablePointer) -> OSStatus
```

## Parameters 

`printSession`  

A pointer to your PMPrintSession variable. On return, the variable refers to a new printing session object. You are responsible for releasing the printing session object with the function PMRelease(_:).

## Return Value

A result code. See Result Codes.

## Discussion

This function allocates memory for a new printing session object in your application’s memory space and sets its reference count to 1. The new printing session object is initialized with information that the printing system uses for a print job.

