

- ProximityReader
-  StoreAndForwardBatch 

Structure

# StoreAndForwardBatch

A structure that stores the data to send to the payment service provider to process.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
struct StoreAndForwardBatch
```

## Overview

The framework invokes these payments using a Store and Forward session.

## Topics

### Structures

struct StoredPaymentCardReadResult

A result structure that represents each payment the framework read using a Store and Forward session.

### Instance Properties

let count: Int

The number of payments this batch includes.

let id: String

The unique identifier for the batch.

let intermediateCertificate: [String]

An array that contains the intermediate certificates that the system uses to sign the leaf certificate.

let leafCertificate: String

The leaf certificate the framework uses to sign this batch.

let payments: [StoreAndForwardBatch.StoredPaymentCardReadResult]

The payments that are part of the batch.

let signature: String

The signature, as a Base64-encoded string, that guarantees the integrity of the batch.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

## Relationships

### Conforms To

- Encodable
- Identifiable
- Sendable

