

- MusicKit
-  MusicUserTokenProvider 

Class

# MusicUserTokenProvider

A class that music requests use to fetch user tokens your app requires to access Apple Music API.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class MusicUserTokenProvider
```

## Topics

### Initializers

init()

Creates a user token provider.

### Instance Methods

func userToken(for: String, options: MusicTokenRequestOptions) async throws -> String

Fetches and returns a user token for Apple Music API.

## Relationships

### Inherited By

- DefaultMusicTokenProvider

## See Also

### Token management

typealias MusicTokenProvider

An object that music requests use to access Apple Music API.

protocol MusicDeveloperTokenProvider

A set of methods that music requests use to access Apple Music API.

struct MusicTokenRequestOptions

Options that music requests pass into token provider methods to fetch a required token for accessing Apple Music API.

enum MusicTokenRequestError

An error that the token provider or music requests can throw upon requesting any token necessary for accessing Apple Music API.

class DefaultMusicTokenProvider

The default token provider that music requests use to access Apple Music API.

