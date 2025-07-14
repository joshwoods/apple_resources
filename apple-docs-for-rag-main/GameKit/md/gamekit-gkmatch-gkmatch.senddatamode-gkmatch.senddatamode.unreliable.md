

- GameKit
- GKMatch
- GKMatch.SendDataMode
-  GKMatch.SendDataMode.unreliable 

Case

# GKMatch.SendDataMode.unreliable

Sends data once even if an error occurs.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
case unreliable
```

## Mentioned in 

Exchanging data between players in real-time games

## Discussion

Use this mode for small packets of data that must arrive quickly to be useful to the recipient. Unreliable data may arrive in a different order than when you sent it.

## See Also

### Modes

case reliable

Sends data continuously until the recipients successfully receive it or the connection times out.

