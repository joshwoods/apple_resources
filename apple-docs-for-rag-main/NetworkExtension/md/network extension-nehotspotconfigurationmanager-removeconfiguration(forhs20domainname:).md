

- Network Extension
- NEHotspotConfigurationManager
-  removeConfiguration(forHS20DomainName:) 

Instance Method

# removeConfiguration(forHS20DomainName:)

Removes a Wi-Fi hotspot configuration, identified by a Hotspot 2.0 domain name, that your app previously added.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func removeConfiguration(forHS20DomainName domainName: String)
```

## Parameters 

`domainName`  

The domain name of the HS 2.0 Wi-Fi network.

## Discussion

Your app can use this method to delete a configuration that it has added, but not a configuration added by another app or by the user. The user can also delete configured networks through Settings \> Wi-Fi.

## See Also

### Removing configuration

func removeConfiguration(forSSID: String)

Removes a Wi-Fi configuration, identified by an SSID, that your app previously added.

