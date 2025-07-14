

- Kernel
- Kernel Enumerations
- Anonymous
-  kIONetworkFeatureSoftwareVlan 

Enumeration Case

# kIONetworkFeatureSoftwareVlan

macOS 10.12+

``` source
kIONetworkFeatureSoftwareVlan = 0x004
```

## Discussion

Set this bit in the value returned by getFeatures() to indicate that the controller can support software based vlan by transmitting and receiving packets 4 bytes longer that normal.

