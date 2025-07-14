

- AppKit
- NSWorkspace
-  localizedDescription(forType:) Deprecated

Instance Method

# localizedDescription(forType:)

Returns the localized description for the specified Uniform Type Identifier (UTI).

macOS 10.5–12.0Deprecated

``` source
func localizedDescription(forType typeName: String) -> String?
```

Deprecated

Use UTType.localizedDescription instead.

## Parameters 

`typeName`  

A string containing the UTI.

## Return Value

An NSString containing the localized description of `typeName`. You may display this string to the user.

## Discussion

You can safely call this method from any thread of your app.

## See Also

### Manipulating Uniform Type Identifier Information

func type(ofFile: String) throws -> String

Returns the uniform type identifier of the specified file, if it can be determined.

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

