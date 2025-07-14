

- SecureElementCredential
- CredentialTransaction
-  CredentialTransaction.Configuration 

Class

# CredentialTransaction.Configuration

An object that provides configuration information for a transaction that the client intends to peform.

SecureElementCredentialSwiftUIiOS 18.1+iPadOS 18.1+

``` source
class Configuration
```

## Mentioned in 

Accessing and using secure element credentials

## Overview

In SwiftUI apps, you fetch a `Configuration` for use in calling the doc://com.apple.documentation/documentation/SwiftUI/View/transactionTask(\_:action) view modifer to perform wired transactions and card emulation. Inside the task closure, call invalidate() on the configuration when you finish your transaction work.

## Topics

### Invalidating a configuration

func invalidate() async throws

Invalidates the configuration and transitions the underlying session state to management.

### Comparing configurations

static func == (CredentialTransaction.Configuration, CredentialTransaction.Configuration) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

## See Also

### Using SwiftUI

func configuration() async throws -> CredentialTransaction.Configuration

Retrieves a transaction configuration related to this session.

