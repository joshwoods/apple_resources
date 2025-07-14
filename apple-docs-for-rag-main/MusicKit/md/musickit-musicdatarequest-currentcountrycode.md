

- MusicKit
- MusicDataRequest
-  currentCountryCode 

Type Property

# currentCountryCode

Fetches the current country code for the user’s Apple Music account.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var currentCountryCode: String { get async throws }
```

## Discussion

The current country code may be useful to construct the URL for a MusicDataRequest because a typical catalog endpoint for Apple Music API requires the inclusion of a country code in the path of the corresponding URL.

