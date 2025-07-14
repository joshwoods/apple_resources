

- StoreKit
- AppStore
-  AppStore.Environment 

Structure

# AppStore.Environment

Constants that represent the App Store server environment.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Environment
```

## Topics

### Getting the environment value

static let production: AppStore.Environment

A value that indicates the production server environment.

static let sandbox: AppStore.Environment

A value that indicates the sandbox server environment.

static let xcode: AppStore.Environment

A value that indicates the StoreKit Testing in Xcode environment.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the environment

let environment: AppStore.Environment

The server environment that signs the app transaction.

