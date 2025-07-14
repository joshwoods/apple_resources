

- SecureElementCredential
-  CredentialSessionWindowSceneEvent 

Enumeration

# CredentialSessionWindowSceneEvent

An event that a credential session sends to a UIKit scene.

SecureElementCredentialUIKitiOS 17.4+iPadOS 17.4+

``` source
enum CredentialSessionWindowSceneEvent
```

## Mentioned in 

Accessing and using secure element credentials

## Topics

### Events

case presentation

The user performs a gesture, such as double-pressing the side button, to present an NFC display.

case readerDetected

The eligible device detects the RF field of an NFC reader.

### Describing the event

var description: String

A textual representation of this instance.

### Encoding and decoding

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Hashing

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Comparing events

static func == (CredentialSessionWindowSceneEvent, CredentialSessionWindowSceneEvent) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable

## See Also

### Handling events

func windowScene(UIWindowScene, didReceiveCredentialSessionWindowSceneEvent: CredentialSessionWindowSceneEvent)

Informs your app that a credential session event initiated a UIKit scene creation.

**Required**

