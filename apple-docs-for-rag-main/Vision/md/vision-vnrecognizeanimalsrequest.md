

- Vision
-  VNRecognizeAnimalsRequest 

Class

# VNRecognizeAnimalsRequest

A request that recognizes animals in an image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class VNRecognizeAnimalsRequest
```

## Overview

Use the knownAnimalIdentifiers(forRevision:) method to determine which animals the request supports.

## Topics

### Accessing the Results

var results: [VNRecognizedObjectObservation]?

The results of the request to recognize animals.

### Identifying Animals

func supportedIdentifiers() throws -> [VNAnimalIdentifier]

Returns the identifiers of the animals that the request detects.

struct VNAnimalIdentifier

An animal identifier string.

class func knownAnimalIdentifiers(forRevision: Int) throws -> [VNAnimalIdentifier]

Returns a list of animal identifiers the recognition algorithm supports for the specified revision.

Deprecated

### Identifying Request Revisions

let VNRecognizeAnimalsRequestRevision2: Int

A constant for specifying revision 2 of the animal recognition request.

let VNRecognizeAnimalsRequestRevision1: Int

A constant for specifying revision 1 of the animal recognition request.

## Relationships

### Inherits From

- VNImageBasedRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

