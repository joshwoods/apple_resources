

- FinanceKit
- FinanceStore
-  FinanceStore.Changes 

Structure

# FinanceStore.Changes

A structure that records changes to the finance store.

iOS 17.4+iPadOS 17.4+

``` source
struct Changes where Model : Identifiable
```

## Topics

### Instance Properties

let deleted: [Model.ID]

An array of model objects identifiers that the framework deleted from the finance store.

let inserted: [Model]

An array of model objects the framework inserted into the finance store.

let newToken: FinanceStore.HistoryToken

An updated history token.

let updated: [Model]

An array of model objects that the framework updated in the finance store.

## Relationships

### Conforms To

- Sendable

