

- Foundation
- NSItemProvider
-  registeredContentTypesForOpenInPlace 

Instance Property

# registeredContentTypesForOpenInPlace

Registered content types that the system can load as open-in-place files.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var registeredContentTypesForOpenInPlace: [UTType] { get }
```

## See Also

### Registering content types

var registeredContentTypes: [UTType]

Registered content types in the order the app registers each type.

func registeredContentTypes(conformingTo: UTType) -> [UTType]

Returns an array of registered content types that conform to a specified content type.

