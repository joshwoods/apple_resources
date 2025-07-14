

- SwiftUI
- Image
-  init(systemName:) 

Initializer

# init(systemName:)

Creates a system symbol image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 11.0+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(systemName: String)
```

## Parameters 

`systemName`  

The name of the system symbol image. Use the SF Symbols app to look up the names of system symbol images.

## Discussion

This initializer creates an image using a system-provided symbol. Use SF Symbols to find symbols and their corresponding names.

To create a custom symbol image from your app’s asset catalog, use init(_:bundle:) instead.

## See Also

### Creating a system symbol image

init(systemName: String, variableValue: Double?)

Creates a system symbol image with a variable value.

