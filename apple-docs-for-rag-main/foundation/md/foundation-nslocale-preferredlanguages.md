

- Foundation
- NSLocale
-  preferredLanguages 

Type Property

# preferredLanguages

An ordered list of the user’s preferred languages.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var preferredLanguages: [String] { get }
```

## Discussion

Users choose a primary language when configuring a device, as described in Reviewing Language and Region Settings. They may also specify one or more secondary languages in order of preference for use when localization is unavailable in a higher priority language. Use this property to obtain the current user’s ordered list of languages, presented as an array of locale identifier strings.

For more information about language localization in your app, see Language and Locale IDs.

