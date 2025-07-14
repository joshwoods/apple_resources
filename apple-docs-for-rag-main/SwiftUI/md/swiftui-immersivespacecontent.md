

- SwiftUI
-  ImmersiveSpaceContent 

Protocol

# ImmersiveSpaceContent

A type that you can use as the content of an immersive space.

visionOS 1.0+

``` source
@MainActor @preconcurrency
protocol ImmersiveSpaceContent
```

## Overview

A type conforming to this protocol inherits `@preconcurrency @MainActor` isolation from the protocol if the conformance is included in the type’s base declaration:

```
struct MyCustomType: Transition {
    // `@preconcurrency @MainActor` isolation by default
}
```

Isolation to the main actor is the default, but it’s not required. Declare the conformance in an extension to opt out of main actor isolation:

```
extension MyCustomType: Transition {
    // `nonisolated` by default
}
```

## Topics

### Creating immersive space content

var body: Self.Body

**Required**

associatedtype Body : ImmersiveSpaceContent

**Required**

## Relationships

### Conforming Types

- ImmersiveSpaceViewContent

## See Also

### Supporting types

struct ImmersiveSpaceViewContent

Immersive space content that uses a SwiftUI view hierarchy as the content.

