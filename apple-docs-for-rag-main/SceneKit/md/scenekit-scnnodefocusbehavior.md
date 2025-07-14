

- SceneKit
-  SCNNodeFocusBehavior 

Enumeration

# SCNNodeFocusBehavior

Options for the focusable states of a SceneKit node.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
enum SCNNodeFocusBehavior
```

## Topics

### Enumeration Cases

case none

Node is not focusable.

case occluding

Node is not focusable and prevents nodes that it visually obscures from becoming focusable.

case focusable

Node is focusable and prevents nodes that it visually obscures from becoming focusable.

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

### Handling UI Focus

var focusBehavior: SCNNodeFocusBehavior

The focus behavior for a node.

