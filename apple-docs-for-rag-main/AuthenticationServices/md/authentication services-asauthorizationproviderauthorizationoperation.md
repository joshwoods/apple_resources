

- Authentication Services
-  ASAuthorizationProviderAuthorizationOperation 

Structure

# ASAuthorizationProviderAuthorizationOperation

A type that represents an authorization operation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+visionOS 1.0+

``` source
struct ASAuthorizationProviderAuthorizationOperation
```

## Topics

### Handling Configuration Removal

static let configurationRemoved: ASAuthorizationProviderAuthorizationOperation

An operation the system invokes when the extension configuration is removed from the system.

### Creating Operations

init(String)

Creates an authorization operation using the specified string value.

init(rawValue: String)

Creates an authorization operation using the specified raw string value.

### Type Properties

static let directRequest: ASAuthorizationProviderAuthorizationOperation

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Parsing the Request

var url: URL

The complete URL of the request, including all components.

var httpHeaders: [String : String]

The HTTP headers of the request.

var httpBody: Data

The HTTP body of the request.

var realm: String

The realm to which the request applies.

var requestedOperation: ASAuthorizationProviderAuthorizationOperation

The operation for the extension to execute.

var authorizationOptions: [AnyHashable : Any]

A collection of options associated with the request.

