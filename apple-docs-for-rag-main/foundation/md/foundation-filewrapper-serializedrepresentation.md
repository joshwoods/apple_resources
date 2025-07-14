

- Foundation
- FileWrapper
-  serializedRepresentation 

Instance Property

# serializedRepresentation

The contents of the file wrapper as an opaque data object.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var serializedRepresentation: Data? { get }
```

## Discussion

This property contains a data object in the format used by the fileContents pasteboard type. This data object is also suitable for passing to init(serializedRepresentation:).

This property may be `nil` if the user modifies the contents of the file system node after you call read(from:options:) or init(url:options:), but before FileWrapper has read the contents of the file. You can use the immediate reading option to reduce the likelihood of this problem.

## See Also

### Related Documentation

init?(serializedRepresentation: Data)

Initializes the receiver as a regular-file file wrapper from given serialized data.

