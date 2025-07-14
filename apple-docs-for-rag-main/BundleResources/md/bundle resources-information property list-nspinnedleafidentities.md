

- Bundle Resources
- Information Property List
-  NSPinnedLeafIdentities 

Property List Key

# NSPinnedLeafIdentities

A list of allowed leaf certificates for a given domain name.

iOS 14.0+iPadOS 14.0+macOS 11.0+visionOS 1.0+

## Details 

Type  

array of dictionaries

## Discussion

Provide an array of dictionaries as the value for this key. Each dictionary in the array contains the SPKI-SHA256-BASE64 key with a value that represents the Base64-encoded SHA-256 digest of an X.509 certificate’s DER-encoded ASN.1 Subject Public Key Info (SPKI) structure.

```
NSPinnedLeafIdentities : Array {
    Dictionary {
        SPKI-SHA256-BASE64 : String
    }
}
```

When making a network connection to a named domain, App Transport Security (ATS) blocks the connection unless it can find the SPKI digest of the leaf certificate presented by the server among the digests in this array. Consider including more than one leaf certificate to allow for server-side configuration changes.

You must include this key or the NSPinnedCAIdentities key or both in each domain-specific NSPinnedDomains subdictionary. If you include both, then both must produce a match.

## Topics

### Key Digests

SPKI-SHA256-BASE64

The digest of an X.509 certificate’s Subject Public Key Info structure.

## See Also

### Identities

NSPinnedCAIdentities

A list of allowed Certificate Authority certificates for a given domain name.

