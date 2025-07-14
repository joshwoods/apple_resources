

- Bundle Resources
- Entitlements
-  com.apple.developer.contacts.notes 

Property List Key

# com.apple.developer.contacts.notes

A Boolean value that indicates whether the app may access the notes in contact entries.

iOS 13.0+iPadOS 13.0+macOS 13.0+visionOS 1.0+

## Details 

Type  

boolean

## Discussion

When your app loads one or more entries from the user’s contacts — for example, by calling the unifiedContacts(matching:keysToFetch:) method — you provide a list of keys specifying the fields to fetch. To request the note field using CNContactNoteKey in iOS 13 or later or macOS 13 or later, your app must have the com.apple.developer.contacts.notes entitlement. When your app tries to fetch notes without the entitlement, it receives an unauthorizedKeys error. Your app only needs the entitlement if it reads or writes notes.

Add the entitlement to your app in the Xcode property list editor. Set the entitlement’s type to Boolean, and the corresponding value to `YES`.

Before you submit an app with this entitlement to the App Store, you need to get permission to use the entitlement. Request permission at https://developer.apple.com/contact/request/contact-note-field.

