

- Network Extension
- NEDNSProxyManager
-  removeFromPreferences(completionHandler:) 

Instance Method

# removeFromPreferences(completionHandler:)

Removes the DNS proxy configuration from the caller’s DNS proxy preferences.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func removeFromPreferences(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
func removeFromPreferences() async throws
```

## Parameters 

`completionHandler`  

A block called when the remove operation completes. If the operation fails, an error instance passed to this block describes the problem. Otherwise, the error is `nil`. See NEDNSProxyManagerError for the list of possible errors.

## Discussion

If you use a device without an installed configuration profile during development, your app can create the DNS proxy configuration from scratch. You first call the loadFromPreferences(completionHandler:) method to retrieve the empty configuration. You then make updates and call the saveToPreferences(completionHandler:) method to store them. To remove the configuration, call the removeFromPreferences(completionHandler:) method. This allows you to restore the device to a clean, unconfigured state.

In a production environment, however, a configuration profile placed in the system by an external process typically provides the baseline DNS proxy configuration. Your app can modify this configuration at runtime using the same load-modify-save steps, but cannot remove the configuration entirely. An attempt to remove the configuration when a configuration profile is present on the device results in a NEDNSProxyManagerError.configurationCannotBeRemoved error.

If the DNS proxy is enabled, it becomes disabled as a result of this call.

## See Also

### Managing the DNS proxy configuration

class func shared() -> NEDNSProxyManager

Returns a singleton DNS proxy manager instance.

func loadFromPreferences(completionHandler: ((any Error)?) -> Void)

Loads the current DNS proxy configuration from the caller’s DNS proxy preferences.

func saveToPreferences(completionHandler: ((any Error)?) -> Void)

Saves the DNS proxy configuration in the caller’s DNS proxy preferences.

