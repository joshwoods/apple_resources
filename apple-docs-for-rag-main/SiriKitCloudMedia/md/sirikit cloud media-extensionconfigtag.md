

- SiriKit Cloud Media
-  ExtensionConfigTag 

Type

# ExtensionConfigTag

A unique identifier for a specific media service configuration.

SiriKit Cloud Media 1.0.2+

``` source
string ExtensionConfigTag
```

## Possible Values 

`/["][ -~]{1000}["]/`  

## Attributes 

Maximum length: `1002`

## Discussion

Change this value whenever anything in your service’s ExtensionConfig changes. Don’t include any personally identifiable information in this value and ensure the value matches the `/["][ -~]{1000}["]/` pattern.

## See Also

### Device Configuration

Configure Your Service Endpoints

Provide configuration details for your media server’s endpoints to a HomePod speaker or an Apple TV.

object ExtensionConfig

Instructions for accessing your media service’s endpoints.

object PlayMediaControlActivity

Options for reporting playback progress.

