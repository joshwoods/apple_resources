

- GameKit
- GKTransportType
-  GKTransportType.unreliable 

Case

# GKTransportType.unreliable

The data is sent once and is not sent again if a transmission error occurs.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
case unreliable
```

## Discussion

Use this for small packets of data that must arrive quickly to be useful to the recipient.

## See Also

### Constants

case reliable

The data is sent continuously until it is successfully received by the intended recipients or the connection times out.

