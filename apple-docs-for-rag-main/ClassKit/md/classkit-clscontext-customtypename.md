

- ClassKit
- CLSContext
-  customTypeName 

Instance Property

# customTypeName

An optional name that the system presents to the user if you choose the custom context type.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 11.0+visionOS 1.0+

``` source
var customTypeName: String? { get set }
```

## Discussion

The system ignores the value of this property unless you set the context’s type property to CLSContextType.custom. If you do set the type name, provide a localized value.

If you use a custom context type but don’t set the type name, the system presents a default, localized string instead.

## See Also

### Managing the context type

var type: CLSContextType

The kind of content a context represents.

func setType(CLSContextType)

Updates the kind of content that a context represents.

enum CLSContextType

The kinds of assignable content a context can contain.

