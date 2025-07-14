

- External Accessory
- EAWiFiUnconfiguredAccessoryBrowserDelegate
-  accessoryBrowser(\_:didFinishConfiguringAccessory:with:) 

Instance Method

# accessoryBrowser(\_:didFinishConfiguringAccessory:with:)

Indicates that the browser has completed configuring the specified accessory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func accessoryBrowser(
    _ browser: EAWiFiUnconfiguredAccessoryBrowser,
    didFinishConfiguringAccessory accessory: EAWiFiUnconfiguredAccessory,
    with status: EAWiFiUnconfiguredAccessoryConfigurationStatus
)
```

**Required**

## Parameters 

`browser`  

The instance of EAWiFiUnconfiguredAccessoryBrowser that is generating the event.

`accessory`  

The EAWiFiUnconfiguredAccessory object whose configuration process has completed.

`status`  

The status of the completed configuration process. See EAWiFiUnconfiguredAccessoryConfigurationStatus for possible values.

## Discussion

This method is called when the system-provided configuration view has been dismissed, revealing the part of the app’s user interface that was visible before the configuration process began. If the configuration was successful, the app can begin communicating with the accessory.

## See Also

### Getting Updates About the Configuration Process

enum EAWiFiUnconfiguredAccessoryConfigurationStatus

Values that represent the state of the configuration process for an EAWiFiUnconfiguredAccessory object.

