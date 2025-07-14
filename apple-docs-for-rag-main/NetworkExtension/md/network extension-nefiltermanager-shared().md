

- Network Extension
- NEFilterManager
-  shared() 

Type Method

# shared()

Access the single instance of `NEFilterManager`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
class func shared() -> NEFilterManager
```

## Return Value

The `NEFilterManager` instance for the calling application.

## See Also

### Managing the filter configuration

func loadFromPreferences(completionHandler: ((any Error)?) -> Void)

Load the filter configuration from the Network Extension preferences.

func saveToPreferences(completionHandler: ((any Error)?) -> Void)

Save the filter configuration in the Network Extension preferences.

func removeFromPreferences(completionHandler: ((any Error)?) -> Void)

Remove the filter configuration from the Network Extension preferences.

