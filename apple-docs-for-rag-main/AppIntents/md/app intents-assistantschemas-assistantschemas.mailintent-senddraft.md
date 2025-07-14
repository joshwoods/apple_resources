

- App Intents
- AssistantSchemas
- AssistantSchemas.MailIntent
-  sendDraft 

Instance Property

# sendDraft

The app intent conforms to the schema for sending an email draft.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var sendDraft: some AssistantSchemas.Intent { get }
```

## Mentioned in 

Making email actions available to Siri and Apple Intelligence

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app intent implementation.

For more information about the `.mail` app intent domain, see Making email actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app intent that conforms to the `.mail.sendDraft` schema:

```
@AssistantIntent(schema: .mail.sendDraft)
struct SendDraftIntent: AppIntent {
    @Parameter
    var target: MailDraftEntity

    @Parameter
    var sendLaterDate: Date?

    func perform() async throws -> some IntentResult {
        .result()
    }
}
```

