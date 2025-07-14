

- Device Management
- Implementing Device Management
-  Simplifying MDM Server Administration for iOS Devices 

Article

# Simplifying MDM Server Administration for iOS Devices

Create a service configuration entry point to your MDM server to access to frequently used information.

## Overview

Add an unauthenticated HTTPS request entry point to your server to make it easier to access useful information about your MDM server. Create the entry point using the endpoint `/MDMServiceConfig`; for example, `https://mdm.example.com/MDMServiceConfig`. The server code should return a UTF-8 JSON-encoded hash (`Content-Type: application/json; charset=UTF8`) with the following values in the body of its response:

`dep_anchor_certs_url`  
The URL a device uses to obtain the certificates required to trust the URL specified by the `dep_enrollment_url` key. This value has the same format as the `anchor_certs` value in the DEP profile, except the body needs to be UTF-8 JSON-encoded for transfer. The decoded body of the response from this URL should be usable in a Device Enrollment Program (DEP) profile under the `anchor_certs` key without any modification.

Provide this URL even if the MDM server doesn’t require additional certificates because it’s using a trusted SSL certificate. However, provide either an empty body (`Content-Length: 0`) or an empty array JSON string (`'[]'`) .

`dep_enrollment_url`  
The URL a device uses to begin MDM enrollment with the MDM server. This is also the URL to use for the `url` key when defining a DEP profile using `https://mdmenrollment.apple.com/profile`.

`trust_profile_url`  
The URL a device uses to obtain a Trust Profile for the MDM server, as a fully-formed `.mobileconfig` profile with only payloads of type `com.apple.security.root`.

Omit this key if the MDM server doesn’t require a Trust Profile because it’s using a trusted SSL certificate. Don’t return a URL that would generate an empty profile.

Tip

Provide a value for `dep_anchor_certs_url` if you provide a value for `dep_enrollment_url`.

### Example of an MDMServiceConfig Request

```
// Format
GET https://mdm.example.com/MDMServiceConfig

// Response body
{    "dep_enrollment_url": "https://mdm.example.com/devicemanagement/mdm/dep_mdm_enroll",
    "dep_anchor_certs_url": "https://mdm.example.com/devicemanagement/mdm/dep_anchor_certs",
    "trust_profile_url": "https://certs.example.com/mdm/trust_profile"
}
```

### Example of the dep_anchor_certs_url Key

```
// Format
GET https://mdm.example.com/devicemanagement/mdm/dep_anchor_certs

// Response body (truncated)
["MIIEKDCCAxCgAwIBAgIEOjznoTALBgkqhkiG9w0BAQswfjEkMCIGA1UEAwwbU3ly \nYWggQ2VydGlmaWNhd...SVVTo9ll1Lv3OJGqBkxPl9TCC\nfYYnArwzlk4qm1tP\n"]
```

### Example of the trust_profile_url Key

```
// Format
GET https://certs.example.com/mdm/trust_profile

// Response body

    PayloadContent

            PayloadContent

            MIIEKDCCAxCgAwIBAgIEOjznoTALBgkqhkiG9w0BAQswfjEkMCIG
            ...
            9TCCfYYnArwzlk4qm1tP

            PayloadDescription
            Installs the Root certificate for Example Corp.
            PayloadDisplayName
            Root certificate for Example Corp
            PayloadIdentifier
            com.apple.ssl.certificate
            PayloadOrganization
            Example Corp 
            PayloadType
            com.apple.security.root
            PayloadUUID
            B90FA650-5A7D-496A-8C84-0D81C9EBCE6E
            PayloadVersion
            1

PayloadDescription
Configures your device to trust the MDM server.
PayloadDisplayName
Trust Profile for Example Corp
PayloadIdentifier
com.apple.config.mdm.example.com.ssl
PayloadScope
System
PayloadType
Configuration
PayloadUUID
94cdf5c0-bde0-0131-1ed5-005056831d08
PayloadVersion
1 

```

## See Also

### Essentials

Managing MDM Connections

Establish or remove a connection between a device and an MDM server.

