

- MusicKit
-  MusicTokenRequestOptions 

Structure

# MusicTokenRequestOptions

Options that music requests pass into token provider methods to fetch a required token for accessing Apple Music API.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct MusicTokenRequestOptions
```

## Topics

### Initializers

init(rawValue: Int)

Creates a new option set from the given raw value.

### Instance Properties

let rawValue: Int

The corresponding value of the raw type.

### Type Aliases

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

The element type of the option set.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let ignoreCache: MusicTokenRequestOptions

An option that indicates the token provider needs to discard any cached token and generate a new token.

### Default Implementations

Equatable Implementations

OptionSet Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Token management

typealias MusicTokenProvider

An object that music requests use to access Apple Music API.

protocol MusicDeveloperTokenProvider

A set of methods that music requests use to access Apple Music API.

class MusicUserTokenProvider

A class that music requests use to fetch user tokens your app requires to access Apple Music API.

enum MusicTokenRequestError

An error that the token provider or music requests can throw upon requesting any token necessary for accessing Apple Music API.

class DefaultMusicTokenProvider

The default token provider that music requests use to access Apple Music API.

