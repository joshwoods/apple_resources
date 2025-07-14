

- Foundation
- NSData
-  write(to:options:) 

Instance Method

# write(to:options:)

Writes the data object’s bytes to the location specified by a given URL.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func write(
    to url: URL,
    options writeOptionsMask: NSData.WritingOptions = []
) throws
```

## Parameters 

`url`  

The location to which to write the receiver’s bytes.

`writeOptionsMask`  

A mask that specifies options for writing the data. Constant components are described in NSData.WritingOptions.

## Discussion

Since at present only `file://` URLs are supported, there is no difference between this method and write(toFile:options:), except for the type of the first argument.

This method may not be appropriate when writing to publicly accessible files. To securely write data to a public location, use FileHandle instead. For more information, seeSecuring File Operations in Secure Coding Guide.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Writing Data to a File

func write(toFile: String, atomically: Bool) -> Bool

Writes the data object’s bytes to the file specified by a given path.

func write(toFile: String, options: NSData.WritingOptions) throws

Writes the data object’s bytes to the file specified by a given path.

func write(to: URL, atomically: Bool) -> Bool

Writes the data object’s bytes to the location specified by a given URL.

struct WritingOptions

Options for methods used to write data objects.

