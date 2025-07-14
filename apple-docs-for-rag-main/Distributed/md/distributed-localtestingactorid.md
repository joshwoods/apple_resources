

- Distributed
-  LocalTestingActorID 

Structure

# LocalTestingActorID

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
struct LocalTestingActorID
```

## Topics

### Operators

static func == (LocalTestingActorID, LocalTestingActorID) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

init(id: String)

init(parse: String)Deprecated

### Instance Properties

var address: StringDeprecated

var hashValue: Int

The hash value.

let id: String

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Local Testing

class LocalTestingDistributedActorSystem

A `DistributedActorSystem` designed for local only testing.

typealias LocalTestingActorAddressDeprecated

struct LocalTestingInvocationEncoder

class LocalTestingInvocationDecoder

struct LocalTestingInvocationResultHandler

