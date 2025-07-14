

- Network
- NWParameters
- NWParameters.ServiceClass
-  NWParameters.ServiceClass.signaling 

Case

# NWParameters.ServiceClass.signaling

A service for low-loss tolerant, inelastic flow, jitter tolerant, bursty but short rate, and variable size connections.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
case signaling
```

## Discussion

Use this for establishing, maintaining, and tearing down a VoIP call.

## See Also

### Service Classes

case bestEffort

A service type to enable Cellular Network Slicing when not setting the other service types.

case background

A service type for high-delay tolerant, high-loss tolerant, elastic flow, and variable size connections.

case interactiveVideo

A service type for low-delay tolerant, very low-loss tolerant, inelastic flow, and constant packet rate connections.

case interactiveVoice

A service type for low-delay tolerant, very low-loss tolerant, inelastic flow, and constant packet rate connections.

case responsiveData

A service type for medium-delay tolerant, elastic and inelastic flow, bursty, and long-lived connections.

