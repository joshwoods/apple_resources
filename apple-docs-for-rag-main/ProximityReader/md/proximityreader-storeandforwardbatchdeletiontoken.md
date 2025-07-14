

- ProximityReader
-  StoreAndForwardBatchDeletionToken 

Structure

# StoreAndForwardBatchDeletionToken

A secure token that you use to delete a Store and Forward batch.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
struct StoreAndForwardBatchDeletionToken
```

## Overview

A `StoreAndForwardBatchDeletionToken` holds the token your payment service provider supplies when they successfully send a batch of Store and Forward payments for processing.

After receiving the raw token data from your provider, create an instance of this structure and pass it to the resolveBatch(batchDeletionToken:) method. When resolving a Store and Forward batch, the PaymentCardReaderStore uses this token to verify that the payments were delivered to the payment service provider and can now be deleted.

## Topics

### Initializers

init(rawValue: String)

Creates a token with the string your payment service provider provides.

### Instance Properties

let rawValue: String

The raw token string your payment service provider supplies.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

