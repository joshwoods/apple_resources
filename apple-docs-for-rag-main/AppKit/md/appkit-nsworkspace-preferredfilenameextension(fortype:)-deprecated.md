

- AppKit
- NSWorkspace
-  preferredFilenameExtension(forType:) Deprecated

Instance Method

# preferredFilenameExtension(forType:)

Returns the preferred filename extension for the specified Uniform Type Identifier (UTI).

macOS 10.5–12.0Deprecated

``` source
func preferredFilenameExtension(forType typeName: String) -> String?
```

Deprecated

Use UTType.preferredFilenameExtension instead.

## Parameters 

`typeName`  

A string containing the UTI.

## Return Value

The appropriate filename extension for `typeName`, or `nil` if no extension could be determined.

## Discussion

You can safely call this method from any thread of your app.

## See Also

### Manipulating Uniform Type Identifier Information

func type(ofFile: String) throws -> String

Returns the uniform type identifier of the specified file, if it can be determined.

Deprecated

func localizedDescription(forType: String) -> String?

Returns the localized description for the specified Uniform Type Identifier (UTI).

Deprecated

func filenameExtension(String, isValidForType: String) -> Bool

Returns whether the specified filename extension is appropriate for the Uniform Type Identifier (UTI).

Deprecated

func type(String, conformsToType: String) -> Bool

Returns a Boolean indicating that the first Uniform Type Identifier (UTI) conforms to the second UTI.

Deprecated

