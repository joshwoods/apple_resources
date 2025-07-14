

- App Intents
- App intent domains
-  Making email actions available to Siri and Apple Intelligence 

Article

# Making email actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s email functionality with Siri and Apple Intelligence.

## Overview

To integrate your app’s email capabilities with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app intent and app entity implementation that Apple Intelligence needs. For example, if your app allows someone to draft an email and send that at a later date and time, use the AssistantIntent(schema:) macro and provide the assistant schema that consists of the `.mail` domain and the sendDraft schema:

```
@AssistantIntent(schema: .mail.sendDraft)
struct SendDraftIntent: AppIntent {
    var target: MailDraftEntity
    var sendLaterDate: Date?

    @MainActor
    func perform() async throws -> some IntentResult {
        return .result()
    }
}
```

To learn more about assistant schemas, see Integrating actions with Siri and Apple Intelligence. For a list of available app intent schemas in the `.mail` domain, see AssistantSchemas.MailIntent.

### Make sure your entity meets requirements

If you use app entities to describe custom data types, annotate the app entity implementation with the AssistantEntity(schema:) macro. This makes sure Siri and Apple Intelligence can understand your data. For example, the intent in the previous section uses `MailDraftEntity`. The following code snippet shows how the `MailDraftEntity` implementation uses the AssistantEntity(schema:) macro:

```
@AssistantEntity(schema: .mail.draft)
struct MailDraftEntity {

    static var defaultQuery = Query()

    struct Query: EntityStringQuery {
        init() {}
        func entities(for identifiers: [MailDraftEntity.ID]) async throws -> [MailDraftEntity] { [] }
        func entities(matching string: String) async throws -> [MailDraftEntity] { [] }
    }

    var displayRepresentation: DisplayRepresentation { "Provide a display representation." }

    let id = UUID()

    var to: [IntentPerson]
    var cc: [IntentPerson]
    var bcc: [IntentPerson]
    var subject: String?
    var body: String?
    var attachments: [IntentFile]
    var account: MailAccountEntity
}
```

The assistant schema for the `MailDraftEntity` consists of the `.mail` domain and the draft schema.

For a list of available app entity schemas in the `.mail` domain, see AssistantSchemas.MailEntity.

## See Also

### Email

protocol MailIntent

Assistant schema conformance for app intents that offer email functionality.

protocol MailEntity

Assistant schema conformance for app entities that describe email.

