

- Device Management
- TopLevel
-  TopLevel.ConsentText 

Device Management Profile

# TopLevel.ConsentText

The dictionary of consent agreements per language.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+Device Assignment ServicesVPP License Management

``` source
object TopLevel.ConsentText
```

## Properties

`ConsentTextItem`

TopLevel.ConsentText.ConsentTextItem

 (Required) 

The dictionary containing a key that consists of the IETF BCP 47 identifier for a language (for example, en or jp) and a value that consists of the agreement localized to that language.

## Topics

### Profiles

object TopLevel.ConsentText.ConsentTextItem

A specific pairing of language code and consent text.

## See Also

### Supporting Objects

object TopLevel.ConsentText.ConsentTextItem

A specific pairing of language code and consent text.

object TopLevel.PayloadContentItem

The payload-specific content for this profile.

