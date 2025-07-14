

- ProximityReader
- VASReadResult
-  VASReadResult.ReadEntry 

Structure

# VASReadResult.ReadEntry

An object containing encrypted data associated with a customer’s loyalty or reward pass.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
struct ReadEntry
```

## Topics

### Getting the customer data

let customerVASData: Data?

The encrypted content of the pass stored in Wallet, which contains the loyalty or reward pass identifier.

### Getting the status word

let status: VASReadResult.ReadEntry.Status

The status word that represents the outcome of the VAS read attempt for this reward pass.

enum Status

Status words that indicate the possible read outcomes.

### Getting the entry ID

let id: String

The merchant identifier you used to retrieve the loyalty program information from Wallet.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

## Relationships

### Conforms To

- Identifiable
- Sendable

## See Also

### Getting the entry details

let entries: [VASReadResult.ReadEntry]

The list of loyalty reward card entries received from the customer.

