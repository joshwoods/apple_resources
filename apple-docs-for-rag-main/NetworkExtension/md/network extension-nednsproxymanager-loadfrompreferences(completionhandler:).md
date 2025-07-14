

- Network Extension
- NEDNSProxyManager
-  loadFromPreferences(completionHandler:) 

Instance Method

# loadFromPreferences(completionHandler:)

Loads the current DNS proxy configuration from the caller’s DNS proxy preferences.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func loadFromPreferences(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
func loadFromPreferences() async throws
```

## Parameters 

`completionHandler`  

A block called when the load operation completes. If the operation fails, an error instance passed to this block describes the problem. Otherwise, the error is `nil`. See NEDNSProxyManagerError for the list of possible errors.

## Discussion

Initially, the DNS proxy configuration comes from a configuration profile stored on the device in a managed environment, as described in Configuration Profile Reference.

When you want to inspect or make changes to the configuration, you call the proxy manager’s loadFromPreferences(completionHandler:) method. This causes the system to load the configuration into the manager’s providerProtocol and isEnabled properties.

If you modify the configuration stored in these properties, you must then call the saveToPreferences(completionHandler:) method to make the changes take effect. Saving the preferences also stores the modified configuration on disk for use the next time the proxy is started or the configuration is loaded.

## See Also

### Managing the DNS proxy configuration

class func shared() -> NEDNSProxyManager

Returns a singleton DNS proxy manager instance.

func saveToPreferences(completionHandler: ((any Error)?) -> Void)

Saves the DNS proxy configuration in the caller’s DNS proxy preferences.

func removeFromPreferences(completionHandler: ((any Error)?) -> Void)

Removes the DNS proxy configuration from the caller’s DNS proxy preferences.

