

- Technotes
-  TN3149: Fetching Contacts change history events 

Article

# TN3149: Fetching Contacts change history events

Learn how to fetch and process the most recent changes to the Contacts database.

## Overview

The Contacts framework has a new fetch request to retrieve information from the user’s Contacts database. A change history fetch request efficiently returns a collection of change history events that describes the contacts and groups added to, deleted from, and updated in the Contacts database. You can fetch all changes in the database or limit the search to changes that have occurred since your last fetch operation. Then, inspect the fetch result to determine what changes have occurred such as a contact was updated or a contact was removed from a group. To fetch change history events in your app, follow these steps:

1.  Adopt the change history event visitor protocol.

2.  Create a change history fetch request.

3.  Configure the change history fetch request

4.  Execute the change history fetch request.

5.  Process a change history event.

6.  Save the starting history token.

Important

Your app needs to obtain permission from the user before accessing Contacts entries. See Requesting Authorization to Access Contacts for details.

## Adopt the change history event visitor protocol

The CNChangeHistoryEvent class encapsulates all possible changes that the system can make to the Contacts database, such as dropping cached information, adding a contact, or updating a group. To receive these changes in your app, create and use a class that conforms to the CNChangeHistoryEventVisitor protocol. Classes adopting this protocol must implement the visitDropEverythingEvent:, visitAddContactEvent:, visitUpdateContactEvent:, and visitDeleteContactEvent: instance methods.

```
```

CNChangeHistoryEventVisitor also provides optional methods such as visitAddMemberToGroupEvent:. Each method provides the change history event associated with the changes. Inspect the properties of the event to detemine the new values or modifications brought to contact properties. For example, visitUpdateContactEvent: provides a CNChangeHistoryUpdateContactEvent object whose contact instance property contains updated information about an existing contact. Compare contact to your app’s cached contact properties to determine what properties were updated.

## Create a change history fetch request

Call CNChangeHistoryFetchRequest to create a change history fetch request.

```
```

The change history fetch request can be configured to fetch a range of change events that have occurred to the Contacts database. The range of events begins with a starting history token, startingToken, and ends with the current state of the database. This starting token has a default value of `nil`. If you provide an existing starting token from a previous change history fetch, the request only returns changes that occurred in history after this token.

```
```

If your token has a `nil` value, is invalid or expired, the fetch request returns a drop event followed by an add event for every contact and group in the Contacts database. The drop event indicates that apps should drop cached information. The token can be persisted between the app launches on the current device.

## Configure a change history fetch request

Each CNChangeHistoryFetchRequest object comes with default values that can affect the result of the operation. CNChangeHistoryFetchRequest provides several properties to update these default values.

The fetch request always returns changes to contacts. Changes to groups are optional. If you want to also fetch group changes, set includeGroupChanges to `YES`. This property indicates whether to add group changes to the fetch result. The default value is `NO`.

```
```

The fetch request returns immutable CNContact and CNGroup objects. To fetch mutable contact and group objects, set mutableObjects to `YES`. This property indicates whether to return mutable objects. The default value is `NO`.

```
```

The fetch request returns contact changes as unified contacts. A unified contact is a synthesized merged result of contacts from different accounts that represent the same person. To fetch individual contact changes, set shouldUnifyResults to `NO`. This property specifies whether to return contact changes for either unified contacts or individual contacts. The default value is `YES`.

```
```

The Contacts framework limits the contact properties that you fetch to the unique identifier when executing a change history fetch request. The request always and primarily returns the CNContactIdentifierKey key. To fetch additional contact properties, update additionalContactKeyDescriptors with contact keys. This property takes an array of key descriptors, CNKeyDescriptor. For example, if you want to fetch the email addresses and family name of contacts in addition to their unique identifiers, add the CNContactEmailAddressesKey and CNContactFamilyNameKey keys to additionalContactKeyDescriptors .

```
```

A transaction author, transactionAuthor, is a string that you provide to identify the author who performs a save request. Transaction authors use reverse-domain-style notation. We recommend using your app’s bundle identifier as the transaction author when your app is saving changes to Contacts.

```
```

You can later filter that author from fetched change history events. The fetch result won’t include changes made by authors you would like to ignore or exclude. To exclude changes made by certain authors, update excludedTransactionAuthors with these authors.

```
```

Note

Transaction authors allow you to filter transactions returned in the fetched change history events. They don’t provide any information about the author responsible for making a given change.

## Execute the change history fetch request

Call enumeratorForChangeHistoryFetchRequest:error: on an instance of CNContactStore to execute the change history fetch request. Pass the created CNChangeHistoryFetchRequest object and a NSError object to the call.

```
```

If the fetch request succeeds, enumeratorForChangeHistoryFetchRequest:error: returns a CNFetchResult object. Process the change history events returned in the value property of CNFetchResult. If the fetch request fails, enumeratorForChangeHistoryFetchRequest:error: returns `nil`.

## Process a change history event

To process a change history event, call acceptEventVisitor: on an instance of a class that conforms to CNChangeHistoryEventVisitor.

```
```

If your app receives a drop everything event, enough has changed since the last time your app fetched the history changes that an incremental sync is no longer possible. Following the drop everything event, your app receives an add event for each contact and group currently in the database. This allows you to implement full syncs and incremental syncs using the same code.

Important

Using isKindOfClass to determine the specific class of a change history event isn’t recommended. Use the protocol instance methods as described in Adopt the change history event visitor protocol.

## Save the starting history token

If the fetch request succeeds, inspect the currentHistoryToken property of CNFetchResult. This property provides the history token for the current fetch request. Your app should save this token, then use it when fetching the next change history events.

```
```

## Revision History

- **2023-06-06** First published.

## See Also

### Latest

TN3182: Adding privacy tracking keys to your privacy manifest

Declare the tracking domains you use in your app or third-party SDK in a privacy manifest.

TN3183: Adding required reason API entries to your privacy manifest

Declare the APIs that can potentially fingerprint devices in your app or third-party SDK in a privacy manifest.

TN3184: Adding data collection details to your privacy manifest

Declare the data your app or third-party SDK collects in a privacy manifest.

TN3181: Debugging an invalid privacy manifest

Identify common configurations that cause unsuccessful privacy manifest validation with the App Store.

TN3180: Reverting to App Store Server Notifications V1

Migrate from version 2 to version 1 of App Store Server Notifications using the Modify an App endpoint.

TN3179: Understanding local network privacy

Learn how local network privacy affects your software.

TN3178: Checking for and resolving build UUID problems

Ensure that every Mach-O image has a UUID, and that every distinct Mach-O image has its own unique UUID.

TN3177: Understanding alternate audio track groups in movie files

Learn how alternate groups collect audio tracks, and how to choose which audio track to use in your app.

TN3111: iOS Wi-Fi API overview

Explore the various Wi-Fi APIs available on iOS and their expected use cases.

TN3176: Troubleshooting Apple Pay payment processing issues

Diagnose errors that occur when processing Apple Pay payments, identify common causes, and explore potential solutions.

TN3175: Diagnosing issues with displaying the Apple Pay button on your website

Diagnose common errors received while displaying the Apple Pay button on your website by identifying the underlying causes, and explore potential solutions.

TN3174: Diagnosing issues with the Apple Pay payment sheet on your website

Diagnose errors received while presenting the Apple Pay payment sheet on your website by identifying the underlying causes of common errors and explore their potential solutions.

TN3173: Troubleshooting issues with your Apple Pay merchant identifier configuration

Diagnose errors due to invalid Apple Pay merchant identifier configurations by identifying the underlying causes of common errors and explore their potential solutions.

TN3168: Making your App Clip available in the App Store

Learn how to configure your App Clip to prevent it from being unavailable in the App Store.

TN3124: Debugging coordinate space issues

Learn techniques to help debug any coordinate space issue.

