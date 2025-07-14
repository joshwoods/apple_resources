

- Network Extension
- NEHotspotHS20Settings
-  domainName 

Instance Property

# domainName

The domain name of a Hotspot 2.0 Wi-Fi Network.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var domainName: String { get }
```

## Discussion

The domain name string may be 1-253 characters, inclusive.

## See Also

### Accessing Hotspot 2.0 properties

var isRoamingEnabled: Bool

A Boolean value indicating whether or not roaming is enabled on a Hotspot 2.0 Wi-Fi network.

var mccAndMNCs: [String]

An array of Mobile Country Code (MCC) and Mobile Network Code (MNC) pairs used for Wi-Fi Hotspot 2.0 negotiation.

var naiRealmNames: [String]

An array of Network Access Identifier (NAI) realm name strings used for Wi-Fi Hotspot 2.0 negotiation.

var roamingConsortiumOIs: [String]

An array of Roaming Consortium Organization (RCO) identifiers used for Wi-Fi Hotspot 2.0 negotiation.

