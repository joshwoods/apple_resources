

- App Intents
- AssistantSchemas
-  AssistantSchemas.MailIntent 

Protocol

# AssistantSchemas.MailIntent

Assistant schema conformance for app intents that offer email functionality.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol MailIntent : AssistantSchemas.Model
```

## Mentioned in 

Making email actions available to Siri and Apple Intelligence

## Topics

### Instance Properties

var archiveMail: some AssistantSchemas.Intent

The app intent conforms to the schema for archiving an email message.

var createDraft: some AssistantSchemas.Intent

The app intent conforms to the schema for creating an email draft.

var deleteDraft: some AssistantSchemas.Intent

The app intent conforms to the schema for deleting an email draft.

var deleteMail: some AssistantSchemas.Intent

The app intent conforms to the schema for deleting email messages.

var forwardMail: some AssistantSchemas.Intent

The app intent conforms to the schema for forwarding an email message.

var replyMail: some AssistantSchemas.Intent

The app intent conforms to the schema for replying to an email message.

var saveDraft: some AssistantSchemas.Intent

The app intent conforms to the schema for saving an email draft.

var sendDraft: some AssistantSchemas.Intent

The app intent conforms to the schema for sending an email draft.

var updateDraft: some AssistantSchemas.Intent

The app intent conforms to the schema for updating an email draft.

var updateMail: some AssistantSchemas.Intent

The app intent conforms to the schema for updating email messages.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.IntentSchema
- AssistantSchemas.IntentSchema

## See Also

### Email

Making email actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s email functionality with Siri and Apple Intelligence.

protocol MailEntity

Assistant schema conformance for app entities that describe email.

