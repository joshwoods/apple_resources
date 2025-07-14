

- Foundation
- NSItemProvider
-  registeredContentTypes 

Instance Property

# registeredContentTypes

Registered content types in the order the app registers each type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var registeredContentTypes: [UTType] { get }
```

## Discussion

You app should register content types in order of fidelity. The system uses content types that appear earlier in the array.

## See Also

### Registering content types

var registeredContentTypesForOpenInPlace: [UTType]

Registered content types that the system can load as open-in-place files.

func registeredContentTypes(conformingTo: UTType) -> [UTType]

Returns an array of registered content types that conform to a specified content type.

