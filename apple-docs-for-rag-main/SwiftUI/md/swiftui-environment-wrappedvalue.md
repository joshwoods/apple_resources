

- SwiftUI
- Environment
-  wrappedValue 

Instance Property

# wrappedValue

The current value of the environment property.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var wrappedValue: Value { get }
```

## Discussion

The wrapped value property provides primary access to the value’s data. However, you don’t access `wrappedValue` directly. Instead, you read the property variable created with the Environment property wrapper:

```
@Environment(\.colorScheme) var colorScheme: ColorScheme

var body: some View {
    if colorScheme == .dark {
        DarkContent()
    } else {
        LightContent()
    }
}
```

