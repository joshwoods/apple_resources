

- AppKit
- NSWorkspace
-  type(\_:conformsToType:) Deprecated

Instance Method

# type(\_:conformsToType:)

Returns a Boolean indicating that the first Uniform Type Identifier (UTI) conforms to the second UTI.

macOS 10.5–12.0Deprecated

``` source
func type(
    _ firstTypeName: String,
    conformsToType secondTypeName: String
) -> Bool
```

Deprecated

Use -\[UTType conformsToType:\] instead.

## Parameters 

`firstTypeName`  

A string containing the UTI that should conform to `secondTypeName`.

`secondTypeName`  

A string containing a UTI.

## Return Value

true if `firstTypeName` conforms to the UTI hierarchy of `secondTypeName`; otherwise, false.

## Discussion

Use this method instead of comparing UTIs for equality. See Uniform Type Identifiers Overview for information about UTI conformance.

This method will always return true if the two strings are equal. Use this method with other type names, including those in the CFBundleTypeName keys of your app’s `Info.plist` file.

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

func filenameExtension(String, isValidForType: String) -> Bool

Returns whether the specified filename extension is appropriate for the Uniform Type Identifier (UTI).

Deprecated

