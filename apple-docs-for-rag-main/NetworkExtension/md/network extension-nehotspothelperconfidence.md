

- Network Extension
-  NEHotspotHelperConfidence 

Enumeration

# NEHotspotHelperConfidence

A type that indicates the hotspot helper’s confidence in its ability to handle the network.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum NEHotspotHelperConfidence
```

## Topics

### Confidence Levels

case high

The helper has high confidence in being able to handle the network.

case low

The helper has some confidence in being able to handle the network.

case none

The helper is unable to handle the network.

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

### Network annotation

func setConfidence(NEHotspotHelperConfidence)

Indicate the level of confidence in being able to handle the network.

func setPassword(String)

Provide the password for a protected network.

