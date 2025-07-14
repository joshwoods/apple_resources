

- ContactProvider
-  ContactItemSyncAnchor 

Structure

# ContactItemSyncAnchor

A snapshot point into enumerating changed contact items.

iOS 18.0+iPadOS 18.0+

``` source
struct ContactItemSyncAnchor
```

## Overview

You can break an enumeration of changes into batches with multiple anchors to reduce the memory constraints on the system. During enumeration, you may update the `generationMarker` and `offset` to reflect progress enumerating the changes as they occurred, possibly across mutiple database generations and how many changes occurred within each database generation.

## Topics

### Creating a sync anchor

init(generationMarker: Data, offset: Int)

Creates a sync anchor with the given generation marker and offset.

### Inspecting sync anchor properties

var generationMarker: Data

A value specific to your data source identifying the database generation you’re enumerating for changes.

var offset: Int

An offset from the anchor’s generation marker.

### Encoding and decoding

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Operators

static func == (ContactItemSyncAnchor, ContactItemSyncAnchor) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable

## See Also

### Ending enumeration

func didFinishEnumeratingChanges(upTo: ContactItemSyncAnchor, moreComing: Bool)

Marks a sync anchor of changed contact items as completed.

**Required**

func didFinishEnumeratingChangesWithError(any Error)

Finishes the change enumeration with an error, indicating failure, to the observer.

**Required**

