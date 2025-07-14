

- TipKit
- TipGroup
-  init(\_:\_:) 

Initializer

# init(\_:\_:)

Creates a tip group with the specified presentation priority.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    _ priority: TipGroup.Priority = .firstAvailable,
    @Tips.GroupBuilder _ builder: () -> [any Tip]
)
```

## Parameters 

`priority`  

Presentation priority of the tips. The default value is firstAvailable.

`builder`  

The tips to display.

