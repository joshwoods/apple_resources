

- Accessibility
-  AXFeatureOverrideSessionManager 

Class

# AXFeatureOverrideSessionManager

A manager class to begin and end accessibility feature override sessions. Multiple override sessions are reconciled by combining the requests, preferring feature enablement. Ending all sessions restores the prior state of Accessibility feature enablement. Your app must be entitled with com.apple.developer.accessibility.merchant-api-control.

iOS 18.2+iPadOS 18.2+

``` source
class AXFeatureOverrideSessionManager
```

## Topics

### Instance Methods

func beginOverrideSession(enabling: AXFeatureOverrideSession.Options, disabling: AXFeatureOverrideSession.Options) throws -> AXFeatureOverrideSession

func end(AXFeatureOverrideSession) throws

### Type Properties

class var sharedInstance: AXFeatureOverrideSessionManager

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

