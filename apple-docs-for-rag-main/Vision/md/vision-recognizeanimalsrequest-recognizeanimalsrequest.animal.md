

- Vision
- RecognizeAnimalsRequest
-  RecognizeAnimalsRequest.Animal 

Enumeration

# RecognizeAnimalsRequest.Animal

An identifier for a recognizable animal.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
enum Animal
```

## Topics

### Getting the animals

case cat

An animal identifier for cats.

case dog

An animal identifier for dogs.

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting a request

var supportedAnimals: [RecognizeAnimalsRequest.Animal]

The collection of animals that the request can detect.

