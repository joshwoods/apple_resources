

- Network Extension
-  NEVPNError 

Structure

# NEVPNError

Information about an error encountered while configuring or using a VPN.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
struct NEVPNError
```

## Topics

### Inspecting error properties

enum Code

Codes that indicate the source of an error.

### Error codes

static var configurationDisabled: NEVPNError.Code

An error code that indicates the VPN configuration associated with the VPN manager isn’t enabled.

static var configurationInvalid: NEVPNError.Code

An error code that indicates the VPN configuration associated with the VPN manager object is invalid.

static var connectionFailed: NEVPNError.Code

An error code that indicates the connection to the VPN server failed.

static var configurationStale: NEVPNError.Code

An error code that indicates another process modfied the VPN configuration since the last time the app loaded the configuration.

static var configurationReadWriteFailed: NEVPNError.Code

An error code that indicates an error occurred while reading or writing the Network Extension preferences.

static var configurationUnknown: NEVPNError.Code

An error code that indicates that unspecified error occurred.

### Type Properties

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

