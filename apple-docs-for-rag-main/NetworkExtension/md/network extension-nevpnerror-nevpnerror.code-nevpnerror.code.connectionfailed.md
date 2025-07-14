

- Network Extension
- NEVPNError
- NEVPNError.Code
-  NEVPNError.Code.connectionFailed 

Case

# NEVPNError.Code.connectionFailed

The connection to the VPN server failed.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
case connectionFailed
```

## See Also

### Error codes

case configurationDisabled

An error code indicating the VPN configuration associated with the VPN manager isn’t enabled.

case configurationInvalid

An error code indicating the VPN configuration associated with the VPN manager object is invalid.

case configurationStale

An error code that indicates another process modfied the VPN configuration since the last time the app loaded the configuration.

case configurationReadWriteFailed

An error code that indicates an error occurred while reading or writing the Network Extension preferences.

case configurationUnknown

An error code that indicates that unspecified error occurred.

