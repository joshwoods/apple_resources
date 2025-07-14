

- App Intents
- AssistantSchemas
- AssistantSchemas.EntitySchema
-  account 

Instance Property

# account

The app entity describes an email account.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var account: some AssistantSchemas.Entity { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app entity implementation.

For more information about the `.mail` app intent domain, see Making email actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app entity that conforms to the `.mail.account` schema:

```
@AssistantEntity(schema: .mail.account)
struct MailAccountEntity: AppEntity {
    struct Query: EntityStringQuery {
        func entities(for identifiers: [MailAccountEntity.ID]) async throws -> [MailAccountEntity] { [] }
        func entities(matching string: String) async throws -> [MailAccountEntity] { [] }
    }

    static var defaultQuery = Query()
    var displayRepresentation: DisplayRepresentation { "Mail Account" }

    let id = UUID()

    @Property
    var name: String

    @Property
    var emailAddress: String
}
```

