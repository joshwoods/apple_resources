

- Video Subscriber Account
- VSUserAccountManager
-  VSUserAccountManager.QueryOptions 

Structure

# VSUserAccountManager.QueryOptions

Constants that represent options you use to fetch a list of user accounts.

iOS 16.4+iPadOS 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+

``` source
struct QueryOptions
```

## Topics

### Query options

static var allDevices: VSUserAccountManager.QueryOptions

A constant that indicates fetching user accounts from all the user’s iCloud devices.

### Initializing query options

init(rawValue: Int)

Creates a query option from an integer value you provide.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Getting user accounts

func userAccounts(options: VSUserAccountManager.QueryOptions) async throws -> [VSUserAccount]

Returns a list of registered user accounts for your app.

