

- Image Playground
-  ImagePlaygroundStyle 

Structure

# ImagePlaygroundStyle

Style options that determine the appearance of generated images.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
struct ImagePlaygroundStyle
```

## Overview

When you create images programmatically, you can ask the system to create images in a particular style. The generative model takes the requested style option and applies it to the content it generates.

## Topics

### Getting the style options

static let animation: ImagePlaygroundStyle

An option that yields animated images.

static let illustration: ImagePlaygroundStyle

An option that yields images in a 2D cartoon style.

static let sketch: ImagePlaygroundStyle

An option that yields images in the style of a hand-drawn sketch.

static var all: [ImagePlaygroundStyle]

An option that allows the creation of images in any style.

### Getting the style identifier

let id: String

A text-based description of the style option.

### Operators

static func == (ImagePlaygroundStyle, ImagePlaygroundStyle) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Identifiable
- Sendable

## See Also

### Platform support

struct ImagePlaygroundConcept

Text elements that specify the content to include in the image.

