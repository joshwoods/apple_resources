

- Automatic Assessment Configuration
- AEAssessmentSession
-  supportsConfigurationUpdates 

Type Property

# supportsConfigurationUpdates

A Boolean that indicates whether the current device or platform supports updating a session’s configuration after the session has begun.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+macOS 14.5+

``` source
class var supportsConfigurationUpdates: Bool { get }
```

## See Also

### Managing session configuration

func update(to: AEAssessmentConfiguration)

Changes the session to use the specified configuration.

var configuration: AEAssessmentConfiguration

The current configuration of the session.

class var supportsMultipleParticipants: Bool

A Boolean that indicates whether the current device or platform supports a configuration with one or more participant applications.

