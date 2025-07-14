

- CarPlay
-  CPVoiceControlTemplate 

Class

# CPVoiceControlTemplate

A template that displays a voice control indicator during audio input.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class CPVoiceControlTemplate
```

## Overview

CarPlay navigation apps must show a voice control indicator during audio input by presenting a voice control template. When creating the template, provide one or more CPVoiceControlState objects. To switch between states, call the activateVoiceControlState(withIdentifier:) method.

## Topics

### Creating a Voice Control Template

init(voiceControlStates: [CPVoiceControlState])

Creates a voice control template with a list of voice control states.

class CPVoiceControlState

A voice control state containing title variants and images for use by a voice control template.

### Activating a State

func activateVoiceControlState(withIdentifier: String)

Changes the template’s state to the one matching the specified identifier.

var activeStateIdentifier: String?

The identifier of the template’s current voice control state.

### Getting Available States

var voiceControlStates: [CPVoiceControlState]

The array of voice control states available to the template.

## Relationships

### Inherits From

- CPTemplate

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Navigation

Integrating CarPlay with Your Navigation App

Configure your navigation app to work with CarPlay by displaying your custom map and directions.

class CPTemplateApplicationDashboardScene

A CarPlay scene that controls your app’s dashboard navigation window.

protocol CPTemplateApplicationDashboardSceneDelegate

The methods for responding to the life-cycle events of your navigation app’s dashboard scene.

class CPMapTemplate

A template that displays a navigation overlay that your app draws on the map.

class CPSearchTemplate

A template that provides the ability to search for a destination and see a list of search results.

