

- SwiftUI
- Group
-  init(content:) 

Initializer

# init(content:)

Creates an instance that generates Rotor content by combining, in order, all the Rotor content specified in the passed-in result builder.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(@AccessibilityRotorContentBuilder content: () -> Content)
```

Available when `Content` conforms to `AccessibilityRotorContent`.

Show all declarations

## Parameters 

`content`  

The result builder that generates Rotor content for the group.

