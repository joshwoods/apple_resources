

- Network Extension
- NEFilterManagerError
-  NEFilterManagerError.configurationStale 

Case

# NEFilterManagerError.configurationStale

An error code that indicates another process modfied the filter configuration since the last time the app loaded the configuration.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
case configurationStale
```

## Discussion

This error also occurs if the app tries to save the filter configuration before loading it from the Network Extension preferences the first time after the app launches.

## See Also

### Error codes

case configurationInvalid

An error code that indicates the filter configuration is invalid.

case configurationDisabled

An error code that indicates the filter configuration isn’t enabled.

case configurationCannotBeRemoved

An error code that indicates removing the configuration isn’t allowed.

case configurationPermissionDenied

An error code that indicates the configuration lacks permission.

case configurationInternalError

An error code that indicates an internal configuration error occurred.

