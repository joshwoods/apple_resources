

- Foundation
- NSAttributedString
-  init(\_:including:) 

Initializer

# init(\_:including:)

Creates a reference-type attributed string from the specified value-type attributed string, including an attribute scope that a key path identifies.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
convenience init(
    _ attrStr: AttributedString,
    including scope: KeyPath
) throws where S : AttributeScope
```

## Parameters 

`attrStr`  

The value-type attributed string that provides the text and attributes of the new object.

`scope`  

A key path that identifies the attribute scope of the attributes in `attrStr`. This can be a nested scope that contains several scopes.

## See Also

### Creating a formatted string

convenience init(AttributedString)

Creates a reference-type attributed string from the specified value-type attributed string.

convenience init&lt;S>(AttributedString, including: S.Type) throws

Creates a reference-type attributed string from the specified value-type attributed string, including an attribute scope.

