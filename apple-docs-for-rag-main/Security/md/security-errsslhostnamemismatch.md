

- Security
-  errSSLHostNameMismatch 

Global Variable

# errSSLHostNameMismatch

The host name you connected with does not match any of the host names allowed by the certificate.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var errSSLHostNameMismatch: OSStatus { get }
```

## Discussion

This is commonly caused by an incorrect value for the kCFStreamSSLPeerName property within the dictionary associated with the stream’s kCFStreamPropertySSLSettings key.

