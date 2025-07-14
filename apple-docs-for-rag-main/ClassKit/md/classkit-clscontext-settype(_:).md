

- ClassKit
- CLSContext
-  setType(\_:) 

Instance Method

# setType(\_:)

Updates the kind of content that a context represents.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func setType(_ type: CLSContextType)
```

## Parameters 

`type`  

A new value for the kind of content that the context represents.

## Discussion

Use this method to change the type property of a context that you’ve already created.

## See Also

### Managing the context type

var type: CLSContextType

The kind of content a context represents.

enum CLSContextType

The kinds of assignable content a context can contain.

var customTypeName: String?

An optional name that the system presents to the user if you choose the custom context type.

