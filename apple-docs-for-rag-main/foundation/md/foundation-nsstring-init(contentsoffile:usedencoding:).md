

- Foundation
- NSString
-  init(contentsOfFile:usedEncoding:) 

Initializer

# init(contentsOfFile:usedEncoding:)

Returns an `NSString` object initialized by reading data from the file at a given path and returns by reference the encoding used to interpret the characters.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    contentsOfFile path: String,
    usedEncoding enc: UnsafeMutablePointer?
) throws
```

## Parameters 

`path`  

A path to a file.

`enc`  

Upon return, if the file is read successfully, contains the encoding used to interpret the file at `path`. For possible values, see NSStringEncoding.

## Return Value

An `NSString` object initialized by reading data from the file named by `path`. The returned object may be different from the original receiver. If the file can’t be opened or there is an encoding error, returns `nil`.

## Discussion

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Creating and Initializing a String from a File

convenience init(contentsOfFile: String, encoding: UInt) throws

Returns an `NSString` object initialized by reading data from the file at a given path using a given encoding.

