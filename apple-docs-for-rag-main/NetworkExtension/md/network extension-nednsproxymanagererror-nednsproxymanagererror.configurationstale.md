

- Network Extension
- NEDNSProxyManagerError
-  NEDNSProxyManagerError.configurationStale 

Case

# NEDNSProxyManagerError.configurationStale

Outdated DNS proxy configuration that needs to be loaded.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
case configurationStale
```

## Discussion

You must load the configuration with a call to loadFromPreferences(completionHandler:) before you can save it.

## See Also

### Enumeration Cases

case configurationInvalid

Invalid DNS proxy configuration that cannot be stored.

case configurationDisabled

Disabled DNS proxy configuration.

case configurationCannotBeRemoved

Unremovable DNS proxy configuration.

