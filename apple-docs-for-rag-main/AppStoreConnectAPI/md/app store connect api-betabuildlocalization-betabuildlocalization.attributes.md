

- App Store Connect API
- BetaBuildLocalization
-  BetaBuildLocalization.Attributes 

Object

# BetaBuildLocalization.Attributes

Attributes that describe a Beta Build Localizations resource.

App Store Connect API 1.0+

``` source
object BetaBuildLocalization.Attributes
```

## Properties

`locale`

`string`

The specified locale. To learn more, see Managing metadata in your app by using locale shortcodes.

`whatsNew`

`string`

A field that describes changes and additions to a build and indicates features you would like your users to test.

## Discussion

Table 1 lists allowed locale values.

| `da`      | Danish                |
|-----------|-----------------------|
| `de-DE`   | German                |
| `el`      | Greek                 |
| `en-AU`   | English (Australia)   |
| `en-CA`   | English (Canada)      |
| `en-GB`   | English (U.K.)        |
| `en-US`   | English (U.S.)        |
| `es-ES`   | Spanish (Spain)       |
| `es-MX`   | Spanish (Mexico)      |
| `fi`      | Finnish               |
| `fr-CA`   | French (Canada)       |
| `fr-FR`   | French                |
| `id`      | Indonesian            |
| `it`      | Italian               |
| `ja`      | Japanese              |
| `ko`      | Korean                |
| `ms`      | Malay                 |
| `nl-NL`   | Dutch                 |
| `no`      | Norwegian             |
| `pt-BR`   | Portuguese (Brazil)   |
| `pt-PT`   | Portuguese (Portugal) |
| `ru`      | Russian               |
| `sv`      | Swedish               |
| `th`      | Thai                  |
| `tr`      | Turkish               |
| `vi`      | Vietnamese            |
| `zh-Hans` | Chinese (Simplified)  |
| `zh-Hant` | Chinese (Traditional) |

## See Also

### Related Documentation

Beta Build Localizations

Beta test information about builds, specific to a locale.

### Objects

object BetaBuildLocalization.Relationships

The relationships you included in the request and those on which you can operate.

