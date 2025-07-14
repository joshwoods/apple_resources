

- Device Management
- TopLevel
- TopLevel.ConsentText
-  TopLevel.ConsentText.ConsentTextItem 

Device Management Profile

# TopLevel.ConsentText.ConsentTextItem

A specific pairing of language code and consent text.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+Device Assignment ServicesVPP License Management

``` source
object TopLevel.ConsentText.ConsentTextItem
```

## Properties

`ANY`

`string`

 (Required) 

The key consisting of the IETF BCP 47 identifier for a language (for example, en or jp) and the value consisting of the agreement localized to that language.

## See Also

### Supporting Objects

object TopLevel.ConsentText

The dictionary of consent agreements per language.

object TopLevel.PayloadContentItem

The payload-specific content for this profile.

