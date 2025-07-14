

- AppKit
- NSWorkspace
-  type(ofFile:) Deprecated

Instance Method

# type(ofFile:)

Returns the uniform type identifier of the specified file, if it can be determined.

macOS 10.5–12.0Deprecated

``` source
func type(ofFile absoluteFilePath: String) throws -> String
```

Deprecated

Use -\[NSURL getResourceValue:forKey:error:\] with NSURLContentTypeKey instead.

## Parameters 

`absoluteFilePath`  

The absolute path of the file.

## Return Value

An `NSString` containing the uniform type identifier of the file at `absoluteFilePath`. If no UTI can be determined the return value is `nil`.

## Discussion

If the file at the specified path is a symbolic link, the type of the symbolic link is returned.

You can safely call this method from any thread of your app.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Manipulating Uniform Type Identifier Information

func localizedDescription(forType: String) -> String?

Returns the localized description for the specified Uniform Type Identifier (UTI).

Deprecated

func preferredFilenameExtension(forType: String) -> String?

Returns the preferred filename extension for the specified Uniform Type Identifier (UTI).

Deprecated

func filenameExtension(String, isValidForType: String) -> Bool

Returns whether the specified filename extension is appropriate for the Uniform Type Identifier (UTI).

Deprecated

func type(String, conformsToType: String) -> Bool

Returns a Boolean indicating that the first Uniform Type Identifier (UTI) conforms to the second UTI.

Deprecated

