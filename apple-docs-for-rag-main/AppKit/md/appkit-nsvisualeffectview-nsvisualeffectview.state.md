

- AppKit
- NSVisualEffectView
-  NSVisualEffectView.State 

Enumeration

# NSVisualEffectView.State

Constants to specify how the material appearance should reflect window activity state.

macOS 10.10+

``` source
enum State
```

## Topics

### Visual Effect View States

case followsWindowActiveState

The backdrop should automatically appear active when the window is active, and inactive when it is not.

case active

The backdrop should always appear active.

case inactive

The backdrop should always appear inactive.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enabling or Disabling the Effect

var state: NSVisualEffectView.State

A value that indicates whether a view has a visual effect applied.

