

- Foundation
- NSException
-  raise(\_:format:arguments:) 

Type Method

# raise(\_:format:arguments:)

Creates and raises an exception with the specified name, reason, and arguments.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func raise(
    _ name: NSExceptionName,
    format: String,
    arguments argList: CVaListPointer
)
```

## Parameters 

`name`  

The name of the exception.

`format`  

A human-readable message string (that is, the exception reason) with conversion specifications for the variable arguments in `argList`.

`argList`  

Variable information to be inserted into the formatted exception reason (in the manner of `vprintf`).

## Discussion

The user-defined dictionary of the generated object is `nil`.

## See Also

### Creating and Raising an NSException Object

init(name: NSExceptionName, reason: String?, userInfo: [AnyHashable : Any]?)

Initializes and returns a newly allocated exception object.

func raise()

Raises the receiver, causing program flow to jump to the local exception handler.

