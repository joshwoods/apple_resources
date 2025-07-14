

- Automatic Assessment Configuration
- AEAssessmentSession
-  configuration 

Instance Property

# configuration

The current configuration of the session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
@NSCopying
var configuration: AEAssessmentConfiguration { get }
```

## Discussion

You configure a session when you create it with the init(configuration:) initializer. You can later change the configuration by calling the update(to:) method. Read the configuration property to obtain the session’s current configuration.

## See Also

### Managing session configuration

func update(to: AEAssessmentConfiguration)

Changes the session to use the specified configuration.

class var supportsMultipleParticipants: Bool

A Boolean that indicates whether the current device or platform supports a configuration with one or more participant applications.

class var supportsConfigurationUpdates: Bool

A Boolean that indicates whether the current device or platform supports updating a session’s configuration after the session has begun.

