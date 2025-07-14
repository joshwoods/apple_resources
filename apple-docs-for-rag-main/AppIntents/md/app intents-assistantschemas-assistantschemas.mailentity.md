

- App Intents
- AssistantSchemas
-  AssistantSchemas.MailEntity 

Protocol

# AssistantSchemas.MailEntity

Assistant schema conformance for app entities that describe email.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol MailEntity : AssistantSchemas.Model
```

## Mentioned in 

Making email actions available to Siri and Apple Intelligence

## Topics

### Instance Properties

var account: some AssistantSchemas.Entity

The app entity describes an email account.

var draft: some AssistantSchemas.Entity

The app entity describes an email draft.

var mailbox: some AssistantSchemas.Entity

The app entity describes an email mailbox.

var message: some AssistantSchemas.Entity

The app entity describes an email message.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.EntitySchema
- AssistantSchemas.EntitySchema

## See Also

### Email

Making email actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s email functionality with Siri and Apple Intelligence.

protocol MailIntent

Assistant schema conformance for app intents that offer email functionality.

