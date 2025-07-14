

- AppKit
- NSWorkspace
-  filenameExtension(\_:isValidForType:) Deprecated

Instance Method

# filenameExtension(\_:isValidForType:)

Returns whether the specified filename extension is appropriate for the Uniform Type Identifier (UTI).

macOS 10.5–12.0Deprecated

``` source
func filenameExtension(
    _ filenameExtension: String,
    isValidForType typeName: String
) -> Bool
```

Deprecated

Use +\[UTType typesWithTag:tagClass:conformingToType:\] to get a list of candidate types, then check if the input type conforms to any of them.

## Parameters 

`filenameExtension`  

A string containing the filename extension.

`typeName`  

A string containing the UTI.

## Return Value

true if `fileNameExtension` is a valid extension for `typeName`; otherwise, false.

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

func preferredFilenameExtension(forType: String) -> String?

Returns the preferred filename extension for the specified Uniform Type Identifier (UTI).

Deprecated

func type(String, conformsToType: String) -> Bool

Returns a Boolean indicating that the first Uniform Type Identifier (UTI) conforms to the second UTI.

Deprecated

