

- Network Extension
- NETunnelProviderError
-  NETunnelProviderError.Code 

Enumeration

# NETunnelProviderError.Code

Error codes that the tunnel provider declares.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
enum Code
```

## Topics

### Error codes

case networkSettingsInvalid

The provided tunnel network settings are invalid.

case networkSettingsCanceled

The request to set or clear the tunnel network settings was canceled.

case networkSettingsFailed

The request to set or clear the tunnel network settings failed.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

