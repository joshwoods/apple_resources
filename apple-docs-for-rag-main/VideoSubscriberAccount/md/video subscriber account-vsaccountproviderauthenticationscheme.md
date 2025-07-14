

- Video Subscriber Account
-  VSAccountProviderAuthenticationScheme 

Structure

# VSAccountProviderAuthenticationScheme

Authentication schemes for account provider requests and responses.

iOSiPadOSmacOStvOSvisionOS

``` source
struct VSAccountProviderAuthenticationScheme
```

## Discussion

If the minimum version your app supports is outside the availability of the VSAccountProviderAuthenticationScheme values, you must create an authentication scheme value using the raw string.

```
let request = VSAccountMetadataRequest()
// ...
if #available(iOS 13.0, *) {
  request.supportedAuthenticationSchemes = [.api]
} else {
  request.supportedAuthenticationSchemes = [VSAccountProviderAuthenticationScheme("API")]
}
```

The following table shows the raw strings for the VSAccountProviderAuthenticationScheme values.

| Scheme | Raw Value |
|--------|-----------|
| saml   | “SAML”    |
| api    | “API”     |

## Topics

### Creating an Authentication Scheme

init(String)

Creates a new authentication scheme with the specified string.

init(rawValue: String)

Creates a new authentication scheme with the specified raw value.

### Authentication Scheme Types

static let saml: VSAccountProviderAuthenticationScheme

Represents a SAML authentication scheme.

static let api: VSAccountProviderAuthenticationScheme

Represents any authentication scheme.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enqueuing Requests

func enqueue(VSAccountMetadataRequest, completionHandler: (VSAccountMetadata?, (any Error)?) -> Void) -> VSAccountManagerResult

Submits a request for subscriber account information.

class VSAccountMetadataRequest

An object that specifies what subscriber account information your app retrieves.

class VSAccountMetadata

A collection of information for a subscriber’s account.

class VSAccountManagerResult

An object that represents a request made for subscriber account information.

class VSAccountProviderResponse

An object that contains the response from the account provider.

