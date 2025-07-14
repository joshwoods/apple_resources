

- Bundle Resources
- Information Property List
-  NSBonjourServices 

Property List Key

# NSBonjourServices

Bonjour service types browsed by the app.

iOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

## Details 

Name  
Bonjour services

Type  

array of strings

## Discussion

The value associated with this key is an array of strings that represent Bonjour service types. Include all service types that your app expects to use. Bonjour service type strings look like `_ipp._tcp`, and `_myservice._udp`, where the first substring identifies the application protocol and the second identifies the transport protocol.

## See Also

### Network

NSAdvertisingAttributionReportEndpoint

The URL where Private Click Measurement and SKAdNetwork send attribution information.

NSAppTransportSecurity

A description of changes made to the default security for HTTP connections.

**Name:** App Transport Security Settings

CKSharingSupported

A Boolean value that indicates your app supports CloudKit Sharing.

