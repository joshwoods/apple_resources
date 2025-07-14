

- GameKit
- GKMatch
- GKMatch.SendDataMode
-  GKMatch.SendDataMode.reliable 

Case

# GKMatch.SendDataMode.reliable

Sends data continuously until the recipients successfully receive it or the connection times out.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
case reliable
```

## Mentioned in 

Exchanging data between players in real-time games

## Discussion

Use this mode when you need guaranteed delivery in the order it’s sent, and the speed isn’t critical.

## See Also

### Modes

case unreliable

Sends data once even if an error occurs.

