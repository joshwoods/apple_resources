

- App Intents
- IntentPerson
-  handle 

Instance Property

# handle

The primary `Handle` used to contact this `IntentPerson`

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var handle: IntentPerson.Handle?
```

## See Also

### Getting identifying information

var aliases: [IntentPerson.Handle]

Other secondary `Handle`s used to contact this `IntentPerson`, if any

var isMe: Bool

Whether this `IntentPerson` represents the owner of the device

var image: DisplayRepresentation.Image?

An image representing this `IntentPerson`

struct Handle

A type that describes a single way to contact a person.

enum ParameterMode

The type of interface to show when someone chooses a parameter that contains information about a person.

