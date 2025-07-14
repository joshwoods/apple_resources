

- Bundle Resources
- Information Property List
-  NSAppTransportSecurity 

Property List Key

# NSAppTransportSecurity

A description of changes made to the default security for HTTP connections.

iOS 9.0+iPadOS 9.0+macOS 10.11+visionOS 1.0+

## Details 

Name  
App Transport Security Settings

Type  

object

## Discussion

On Apple platforms, a networking feature called App Transport Security (ATS) improves privacy and data integrity for all apps and app extensions. ATS requires that all HTTP connections made with the URL Loading System—typically using the URLSession class—use HTTPS. It further imposes extended security checks that supplement the default server trust evaluation prescribed by the Transport Layer Security (TLS) protocol. ATS blocks connections that fail to meet minimum security specifications. For additional details, see Preventing Insecure Network Connections.

You can circumvent or augment these protections by adding the NSAppTransportSecurity key to your app’s Information Property List file and providing an ATS configuration dictionary as the value. For example, you can:

- Allow insecure loads for web views while maintaining ATS protections elsewhere in your app using the NSAllowsArbitraryLoadsInWebContent key.

- Enable additional security features like Certificate Transparency using the NSRequiresCertificateTransparency key, or Certificate Pinning using the NSPinnedDomains key.

- Reduce or remove security requirements for communication with particular servers using the NSExceptionDomains key.

Important

Always look for ways to improve server security before adding ATS exceptions. Loosening ATS restrictions reduces the security of your app.

All keys in the ATS configuration dictionary are optional, with default values that are suitable for most apps. Keys that define global exceptions apply to all network connections made by your app, except connections to domains specified in the NSExceptionDomains sub-dictionary. That sub-dictionary allows you to separately manage settings for individual domains.

### Versioning

ATS operates by default for apps linked against the iOS 9.0 or macOS 10.11 SDKs or later. When you link your app against an older SDK, ATS is disabled no matter which version of operating system your app runs on.

If you specify a value for any of the global exceptions besides NSAllowsArbitraryLoads, then the ATS behavior depends on the version of the OS on which your app runs:

iOS 9.0 or macOS 10.11  
ATS uses the NSAllowsArbitraryLoads value that you set, or NO by default, and ignores the other global exceptions.

iOS 10.0 or later or macOS 10.12 or later  
ATS ignores the NSAllowsArbitraryLoads value that you set and instead obeys the other key or keys.

This behavior enables you to manage differences between OS versions. You provide a coarse exception (NSAllowsArbitraryLoads) for older versions, and a more targeted exception, like NSAllowsArbitraryLoadsInWebContent, for when it’s available.

## Topics

### Global Exceptions

NSAllowsArbitraryLoads

A Boolean value indicating whether App Transport Security restrictions are disabled for all network connections.

**Name:** Allow Arbitrary Loads

NSAllowsArbitraryLoadsForMedia

A Boolean value indicating whether all App Transport Security restrictions are disabled for requests made using the AV Foundation framework.

**Name:** Allows Arbitrary Loads for Media

NSAllowsArbitraryLoadsInWebContent

A Boolean value indicating whether all App Transport Security restrictions are disabled for requests made from web views.

**Name:** Allow Arbitrary Loads in Web Content

NSAllowsLocalNetworking

A Boolean value that indicates whether to allow local resources to load.

**Name:** Allows Local Networking

### Domain-Specific Exceptions

NSExceptionDomains

Custom App Transport Security (ATS) configurations for named domains.

**Name:** Exception Domains

### Certificate Pinning

NSPinnedDomains

A collection of certificates that App Transport Security expects when connecting to named domains.

## See Also

### Related Documentation

Preventing Insecure Network Connections

Enforce secure network links in your app by relying on App Transport Security.

### Network

NSAdvertisingAttributionReportEndpoint

The URL where Private Click Measurement and SKAdNetwork send attribution information.

NSBonjourServices

Bonjour service types browsed by the app.

**Name:** Bonjour services

CKSharingSupported

A Boolean value that indicates your app supports CloudKit Sharing.

