

- AppKit
- NSApplication
-  NSApplication.OcclusionState 

Structure

# NSApplication.OcclusionState

This constant indicates whether at least part of any window owned by this app is visible.

macOS 10.9+

``` source
struct OcclusionState
```

## Topics

### Constants

static var visible: NSApplication.OcclusionState

If set, at least part of any window owned by this app is visible.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Getting the Occlusion State

var occlusionState: NSApplication.OcclusionState

The occlusion state of the app.

