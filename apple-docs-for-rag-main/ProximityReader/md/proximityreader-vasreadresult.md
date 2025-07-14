

- ProximityReader
-  VASReadResult 

Structure

# VASReadResult

The result of a request to read loyalty card information.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
struct VASReadResult
```

## Mentioned in 

Accepting loyalty passes from Wallet

## Overview

A `VASReadResult` object contains the encrypted loyalty card information from the customer. Typically, you receive this object only after calling the readVAS(_:) or readPaymentCard(_:vasRequest:stopOnVASResult:) method of PaymentCardReaderSession.

## Topics

### Creating a read result structure

init(id: String, entries: [VASReadResult.ReadEntry])

Creates a new result object with the specified identifier and customer entries.

Deprecated

### Getting the entry details

let entries: [VASReadResult.ReadEntry]

The list of loyalty reward card entries received from the customer.

struct ReadEntry

An object containing encrypted data associated with a customer’s loyalty or reward pass.

### Getting the result ID

let id: String

A unique identifier string for the requested read operation.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

## Relationships

### Conforms To

- Identifiable
- Sendable

## See Also

### Loyalty card requests

Accepting loyalty passes from Wallet

Set up the necessary components so your app can begin using Tap to Pay on iPhone to read and issue loyalty passes.

class VASRequest

A request to read a contactless loyalty card and retrieve loyalty program identifiers for the person.

