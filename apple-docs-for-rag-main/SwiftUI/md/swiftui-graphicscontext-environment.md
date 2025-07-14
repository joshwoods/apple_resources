

- SwiftUI
- GraphicsContext
-  environment 

Instance Property

# environment

The environment associated with the graphics context.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var environment: EnvironmentValues { get }
```

## Discussion

SwiftUI initially sets this to the environment of the context’s enclosing view. The context uses values like display resolution and the color scheme from the environment to resolve types like Image and Color. You can also access values stored in the environment for your own purposes.

