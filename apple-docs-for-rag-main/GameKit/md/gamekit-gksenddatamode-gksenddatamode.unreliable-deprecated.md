

- GameKit
- GKSendDataMode
-  GKSendDataMode.unreliable Deprecated

Case

# GKSendDataMode.unreliable

The data is sent once and is not sent again if a transmission error occurred.

macOS 10.8–10.10DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
case unreliable
```

Deprecated

No longer supported

## Discussion

Data transmitted unreliably may be received out of order by recipients. Use this for small packets of data that must arrive quickly to be useful to the recipient.

## See Also

### Constants

case reliable

The data is sent continuously until it is successfully received by the intended recipients or the connection times out.

Deprecated

