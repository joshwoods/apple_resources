

- SceneKit
-  SCNReferenceLoadingPolicy 

Enumeration

# SCNReferenceLoadingPolicy

Options for when to load the reference node’s content, used by the loadingPolicy property.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum SCNReferenceLoadingPolicy
```

## Topics

### Constants

case immediate

Load the node’s external content immediately when the reference node is unarchived.

case onDemand

Load the node’s external comment only when the load() method is called.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

