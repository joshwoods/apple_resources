

- AVFoundation
- AVContentKey
-  externalContentProtectionStatus 

Instance Property

# externalContentProtectionStatus

The external protection status for the content key based on all attached displays.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+

``` source
var externalContentProtectionStatus: AVExternalContentProtectionStatus { get }
```

## Discussion

This property isn’t key-value observable. Instead, use the contentKeySession(_:externalProtectionStatusDidChangeFor:) delegate method to monitor changes to this value.

## See Also

### Inspecting protection status

func revoke()

