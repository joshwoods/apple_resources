

- Network Extension
- NEHotspotConfigurationManager
-  removeConfiguration(forSSID:) 

Instance Method

# removeConfiguration(forSSID:)

Removes a Wi-Fi configuration, identified by an SSID, that your app previously added.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 7.0+

``` source
func removeConfiguration(forSSID SSID: String)
```

## Parameters 

`SSID`  

A string of 1-32 characters.

## Discussion

Your app can use this method to delete a configuration that it has added, but not a configuration added by another app or by the user. The user can also delete configured networks through Settings \> Wi-Fi.

## See Also

### Removing configuration

func removeConfiguration(forHS20DomainName: String)

Removes a Wi-Fi hotspot configuration, identified by a Hotspot 2.0 domain name, that your app previously added.

