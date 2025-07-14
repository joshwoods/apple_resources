

- Authentication Services
-  ASPublicKeyCredentialClientData 

Structure

# ASPublicKeyCredentialClientData

iOS 17.4+iPadOS 17.4+Mac Catalyst 16.6+macOS 13.5+

``` source
struct ASPublicKeyCredentialClientData
```

## Topics

### Initializers

init(challenge: Data, origin: String, topOrigin: String?, crossOrigin: ASPublicKeyCredentialClientData.CrossOriginValue?)

### Instance Properties

var challenge: Data

var crossOrigin: ASPublicKeyCredentialClientData.CrossOriginValue?

var origin: String

var topOrigin: String?

### Enumerations

enum CrossOriginValue

## Relationships

### Conforms To

- Sendable

