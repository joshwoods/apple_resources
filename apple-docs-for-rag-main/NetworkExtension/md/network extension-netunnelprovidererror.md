

- Network Extension
-  NETunnelProviderError 

Structure

# NETunnelProviderError

An error that the tunnel provider encounters.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
struct NETunnelProviderError
```

## Topics

### Error information

enum Code

Error codes that the tunnel provider declares.

### Error codes

static var networkSettingsInvalid: NETunnelProviderError.Code

The provided tunnel network settings are invalid.

static var networkSettingsCanceled: NETunnelProviderError.Code

The request to set or clear the tunnel network settings was canceled.

static var networkSettingsFailed: NETunnelProviderError.Code

The request to set or clear the tunnel network settings failed.

### Type Properties

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

