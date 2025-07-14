

- Network
- NWParameters
-  applicationService 

Type Property

# applicationService

The default parameters for connecting with other, local devices that are running your app.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
final class var applicationService: NWParameters { get }
```

## Discussion

The default parameters set up an encrypted connection with another device on the local network. You can use these parameters as-is, or you can add a NWProtocolFramer to provide application-level messaging support.

