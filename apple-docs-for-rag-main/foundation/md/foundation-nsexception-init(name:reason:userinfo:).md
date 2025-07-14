

- Foundation
- NSException
-  init(name:reason:userInfo:) 

Initializer

# init(name:reason:userInfo:)

Initializes and returns a newly allocated exception object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    name aName: NSExceptionName,
    reason aReason: String?,
    userInfo aUserInfo: [AnyHashable : Any]? = nil
)
```

## Parameters 

`aName`  

The name of the exception.

`aReason`  

A human-readable message string summarizing the reason for the exception.

`aUserInfo`  

A dictionary containing user-defined information relating to the exception

## Return Value

The created `NSException` object or `nil` if the object couldn’t be created.

## Discussion

This is the designated initializer.

## See Also

### Creating and Raising an NSException Object

class func raise(NSExceptionName, format: String, arguments: CVaListPointer)

Creates and raises an exception with the specified name, reason, and arguments.

func raise()

Raises the receiver, causing program flow to jump to the local exception handler.

