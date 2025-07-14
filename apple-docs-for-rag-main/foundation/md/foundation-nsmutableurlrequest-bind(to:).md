

- Foundation
- NSMutableURLRequest
-  bind(to:) 

Instance Method

# bind(to:)

Binds a URL request to the network interface associated with the hotspot helper command instance.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func bind(to command: NEHotspotHelperCommand)
```

## Parameters 

`command`  

The hotspot helper command to bind the request to.

## Discussion

Apps that participate in joining Wi-Fi hotspot networks use the APIs in the Network Extension framework to authenticate with hotspots. Ordinarily, URLSession will use the default interface, which may be WWAN. By binding to a hotspot helper command, you force a request to use Wi-Fi to communicate with the hotspot.

## See Also

### Related Documentation

Network Extension

Customize and extend core networking features.

