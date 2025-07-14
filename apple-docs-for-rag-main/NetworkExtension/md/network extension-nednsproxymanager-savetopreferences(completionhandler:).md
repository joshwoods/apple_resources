

- Network Extension
- NEDNSProxyManager
-  saveToPreferences(completionHandler:) 

Instance Method

# saveToPreferences(completionHandler:)

Saves the DNS proxy configuration in the caller’s DNS proxy preferences.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func saveToPreferences(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
func saveToPreferences() async throws
```

## Parameters 

`completionHandler`  

A block called when the save operation completes. If the operation fails, an error instance passed to this block describes the problem. Otherwise, the error is `nil`. See NEDNSProxyManagerError for the list of possible errors.

## Discussion

If you alter the DNS proxy configuration that you load into the proxy manager’s properties using a call to the loadFromPreferences(completionHandler:) method, you must then call the saveToPreferences(completionHandler:) method to make the changes take effect. Saving also stores the modified configuration for the next time the proxy is started or the configuration loaded.

Trying to save preferences before loading them produces an error.

If the DNS proxy is enabled, it becomes active as a result of this call.

## See Also

### Managing the DNS proxy configuration

class func shared() -> NEDNSProxyManager

Returns a singleton DNS proxy manager instance.

func loadFromPreferences(completionHandler: ((any Error)?) -> Void)

Loads the current DNS proxy configuration from the caller’s DNS proxy preferences.

func removeFromPreferences(completionHandler: ((any Error)?) -> Void)

Removes the DNS proxy configuration from the caller’s DNS proxy preferences.

