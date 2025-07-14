

- Network Extension
- NEDNSProxyManager
-  shared() 

Type Method

# shared()

Returns a singleton DNS proxy manager instance.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class func shared() -> NEDNSProxyManager
```

## Return Value

The NEDNSProxyManager instance for the app.

## Discussion

Each app is allowed to create a single DNS proxy manager. The shared() type method returns a singleton NEDNSProxyManager instance that your app can use to manage any DNS proxy instances that it creates.

## See Also

### Managing the DNS proxy configuration

func loadFromPreferences(completionHandler: ((any Error)?) -> Void)

Loads the current DNS proxy configuration from the caller’s DNS proxy preferences.

func saveToPreferences(completionHandler: ((any Error)?) -> Void)

Saves the DNS proxy configuration in the caller’s DNS proxy preferences.

func removeFromPreferences(completionHandler: ((any Error)?) -> Void)

Removes the DNS proxy configuration from the caller’s DNS proxy preferences.

