

- App Intents
- DisplayRepresentation
- DisplayRepresentation.Image
-  init(systemName:tintColor:symbolConfiguration:) 

Initializer

# init(systemName:tintColor:symbolConfiguration:)

Creates an image object backed by the given SF Symbol name, with optional configuration options.

AppIntentsUIKitiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init?(
    systemName name: String,
    tintColor: UIColor? = nil,
    symbolConfiguration: UIImage.SymbolConfiguration? = nil
)
```

## Parameters 

`systemName`  

Name of the SF Symbol

`tintColor`  

An optional UIColor to tint the icon

`symbolConfiguration`  

An optional symbol configuration

