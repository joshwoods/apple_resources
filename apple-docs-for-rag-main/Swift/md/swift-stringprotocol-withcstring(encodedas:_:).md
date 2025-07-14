

- Swift
- StringProtocol
-  withCString(encodedAs:\_:) 

Instance Method

# withCString(encodedAs:\_:)

Calls the given closure with a pointer to the contents of the string, represented as a null-terminated sequence of code units.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func withCString(
    encodedAs targetEncoding: Encoding.Type,
    _ body: (UnsafePointer) throws -> Result
) rethrows -> Result where Encoding : _UnicodeEncoding
```

**Required**

## Parameters 

`targetEncoding`  

The encoding in which the code units should be interpreted.

`body`  

A closure with a pointer parameter that points to a null-terminated sequence of code units. If `body` has a return value, that value is also used as the return value for the `withCString(encodedAs:_:)` method. The pointer argument is valid only for the duration of the method’s execution.

## Return Value

The return value, if any, of the `body` closure parameter.

## Discussion

The pointer passed as an argument to `body` is valid only during the execution of `withCString(encodedAs:_:)`. Do not store or return the pointer for later use.

