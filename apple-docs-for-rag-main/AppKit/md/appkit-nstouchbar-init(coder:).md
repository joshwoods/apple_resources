

- AppKit
- NSTouchBar
-  init(coder:) 

Initializer

# init(coder:)

Creates a Touch Bar object from a coder object provided by a storyboard or NIB file.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
init?(coder: NSCoder)
```

## Return Value

A fully initialized Touch Bar object, or `nil` if the coder doesn’t define a Touch Bar object.

## See Also

### Creating a bar

init()

Creates a Touch Bar object.

