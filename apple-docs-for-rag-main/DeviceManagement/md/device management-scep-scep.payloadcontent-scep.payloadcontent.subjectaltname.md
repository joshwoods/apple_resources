

- Device Management
- SCEP
- SCEP.PayloadContent
-  SCEP.PayloadContent.SubjectAltName 

Device Management Profile

# SCEP.PayloadContent.SubjectAltName

An optional dictionary that provides values required by the CA for issuing a certificate.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 3.0+Device Assignment ServicesVPP License Management

``` source
object SCEP.PayloadContent.SubjectAltName
```

## Properties

`dNSName`

`string`

The DNS name.

`ntPrincipalName`

`string`

The NT principal name.

`rfc822Name`

`string`

The RFC 822 (email address) string.

`uniformResourceIdentifier`

`string`

The Uniform Resource Identifier.

## Discussion

You can specify a single string or an array of strings for each key. The values you specify depend on the CA you’re using but might include DNS name, URL, or email values. For an example, see the Example SCEP Configuration Profile or Over-the-Air Profile Delivery and Configuration.

## See Also

### Supporting Objects

object SCEP.PayloadContent

The SCEP dictionary.

