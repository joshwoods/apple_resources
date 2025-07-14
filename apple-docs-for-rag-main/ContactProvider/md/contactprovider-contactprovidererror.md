

- ContactProvider
-  ContactProviderError 

Enumeration

# ContactProviderError

Errors thrown by the Contact Provider framework.

iOS 18.0+iPadOS 18.0+

``` source
enum ContactProviderError
```

## Topics

### Availability errors

case featureNotAvailable

The extension can’t run because the feature isn’t available.

case deniedByUser

The person using the app denied the action.

### Configuration errors

case extensionNotFound

The framework couldn’t discover the app’s extension.

### Capacity errors

case itemsLimitReached

Limit of items has been reached.

### Enumeration errors

case cannotEnumerate

The extension is unable to enumerate.

case enumerationTimeout

The extension enumeration timed out.

### Expiration errors

case pageExpired

The page expired and is no longer valid.

case changeAnchorExpired

The change anchor expired and is no longer valid.

### Invalidation errors

case extensionInvalidated

The app invalidated the extension while it was enumerating content or changes.

case extensionInvalidateTimeout

The extension invalidate operation timed out.

### Hashing

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Enumeration Cases

case domainNotRegistered

The domain has not been registered.

### Default Implementations

CustomNSError Implementations

Equatable Implementations

Error Implementations

LocalizedError Implementations

## Relationships

### Conforms To

- Copyable
- CustomNSError
- Equatable
- Error
- Hashable
- LocalizedError
- Sendable

