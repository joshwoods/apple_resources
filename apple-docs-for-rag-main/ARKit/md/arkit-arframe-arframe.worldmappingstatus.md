

- ARKit
- ARFrame
-  ARFrame.WorldMappingStatus 

Enumeration

# ARFrame.WorldMappingStatus

A value describing the world mapping status for the area visible in a given frame.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
enum WorldMappingStatus
```

## Topics

### Enumeration Cases

case extending

World tracking has mapped recently visited areas, but is still mapping around the current device position.

case limited

World tracking has not yet sufficiently mapped the area around the current device position.

case mapped

World tracking has adequately mapped the visible area.

case notAvailable

No world map is available.

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

### Checking world-mapping status

var worldMappingStatus: ARFrame.WorldMappingStatus

The feasibility of generating or relocalizing a world map for this frame.

