

- dnssd
-  kDNSServiceProperty_DaemonVersion 

Global Variable

# kDNSServiceProperty_DaemonVersion

The daemon version property.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var kDNSServiceProperty_DaemonVersion: String { get }
```

## Discussion

When requesting kDNSServiceProperty_DaemonVersion, the result pointer must point to a 32-bit unsigned integer, and the size parameter must be set to sizeof(uint32_t).

On return, the 32-bit unsigned integer contains the version number, formatted as follows:

Major part of the build number \* 10000 +

minor part of the build number \* 100

For example, OS X 10.4.9 has mDNSResponder-108.4, which would be represented as version 1080400. This allows applications to do simple greater-than and less-than comparisons: e.g. an application that requires at least mDNSResponder-108.4 can check:

```

   if (version >= 1080400) ...

```

Example usage:

```

 uint32_t version;
 uint32_t size = sizeof(version);
 DNSServiceErrorType err = DNSServiceGetProperty(kDNSServiceProperty_DaemonVersion, &version, &size);
 if (!err) printf("Bonjour version is %d.%d\n", version / 10000, version / 100 % 100);

```

## See Also

### Constants

var DNS_SD_ORIGINAL_ENCODING_VERSION_NUMBER_MAX: Int32

let kDNSServiceAttributeAAAAFallback: &lt;&lt;error type>>

var kDNSServiceInterfaceIndexAny: Int32

var kDNSServiceInterfaceIndexBLE: UInt32

var kDNSServiceInterfaceIndexInfra: UInt32

var kDNSServiceInterfaceIndexLocalOnly: UInt32

var kDNSServiceInterfaceIndexP2P: UInt32

var kDNSServiceInterfaceIndexUnicast: UInt32

var kDNSServiceMaxDomainName: Int32

var kDNSServiceMaxServiceName: Int32

