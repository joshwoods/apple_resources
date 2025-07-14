

- Kernel
- Kernel Enumerations
- Anonymous
-  kIONetworkFeatureHardwareVlan 

Enumeration Case

# kIONetworkFeatureHardwareVlan

macOS 10.12+

``` source
kIONetworkFeatureHardwareVlan = 0x002
```

## Discussion

Set this bit in the value returned by getFeatures() to indicate the controller supports hardware stripping and stuffing of 802.1q vlan tags. If the controller supports this feature it must enable it when initializing so that all received packets delivered to higher layers have the tag stripped. The controller should use setVlanTag() to provide the tag information out of band.

