

- System
- FilePath
-  withPlatformString(\_:) 

Instance Method

# withPlatformString(\_:)

Calls the given closure with a pointer to the contents of the file path, represented as a null-terminated platform string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func withPlatformString(_ body: (UnsafePointer) throws -> Result) rethrows -> Result
```

## Parameters 

`body`  

A closure with a pointer parameter that points to a null-terminated platform string. If `body` has a return value, that value is also used as the return value for this method.

## Return Value

The return value, if any, of the `body` closure parameter.

## Discussion

The pointer passed as an argument to `body` is valid only during the execution of this method. Don’t try to store the pointer for later use.

