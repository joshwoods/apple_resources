

- Network Extension
- NEDNSProxyManagerError
-  NEDNSProxyManagerError.configurationCannotBeRemoved 

Case

# NEDNSProxyManagerError.configurationCannotBeRemoved

Unremovable DNS proxy configuration.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
case configurationCannotBeRemoved
```

## Discussion

This error occurs if you attempt to use a call to the removeFromPreferences(completionHandler:) method to remove the DNS proxy configuration when an installed configuration profile specifies a baseline DNS proxy configuration. You can only call the removal method in a development environment where no configuration profile exists.

## See Also

### Enumeration Cases

case configurationInvalid

Invalid DNS proxy configuration that cannot be stored.

case configurationDisabled

Disabled DNS proxy configuration.

case configurationStale

Outdated DNS proxy configuration that needs to be loaded.

