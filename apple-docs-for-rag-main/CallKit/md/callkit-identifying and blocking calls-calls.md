

- CallKit
-  Identifying and blocking calls 

Article

# Identifying and blocking calls

Create a Call Directory app extension to identify and block incoming callers by their phone number.

## Overview

Use the Call Directory app extension to manage callers by their phone number. The system communicates with the app extension and checks a person’s contacts and block lists to identify callers.

Note

The CXCallDirectoryPhoneNumber type represents phone numbers in a Call Directory app extension, and consists of a country calling code (such as `1` for the United States) followed by a sequence of digits.

### Create a Call Directory app extension

You can create a Call Directory app extension for your containing app by adding a new project target and selecting the Call Directory Extension template under Application Extension.

You set up both identification and blocking of incoming calls in the implementation of the beginRequest(with:) method of the CXCallDirectoryProvider subclass of your Call Directory app extension. The system calls this method when it launches the app extension.

For more information about how app extensions work, see App extensions.

### Identify incoming callers

When a phone receives an incoming call, the system first checks the person’s contacts to find a matching phone number. If there’s no match, the system then checks your app’s Call Directory app extension to find a matching entry to identify the phone number. This is useful for apps that maintain a contact list that’s separate from the system contacts, such as for a social network, or for identifying incoming calls that may initiate from within the app, such as for customer service support or a delivery notification.

For example, consider a person who is friends with Maria in a social networking app, but who doesn’t have her phone number in their contacts. The social networking app has a Call Directory app extension, which downloads and adds the phone numbers of all of the person’s friends. Because of this, when there’s an incoming call from Maria, the system displays something like *(App Name) Caller ID: Maria Ruiz* rather than *Unknown Caller*.

To provide identifying information about incoming callers, you use the addIdentificationEntry(withNextSequentialPhoneNumber:label:) method in the implementation of beginRequest(with:).

- Swift
- Objective-C

```
class CustomCallDirectoryProvider: CXCallDirectoryProvider {
    override func beginRequest(with context: CXCallDirectoryExtensionContext) {
        let labelsKeyedByPhoneNumber: [CXCallDirectoryPhoneNumber: String] = [ … ]
        for (phoneNumber, label) in labelsKeyedByPhoneNumber.sorted(by: 

```
```

Because the system calls this method only when it launches the app extension and not for each individual call, you need to specify call identification information all at once. For example, you can’t make a request to a web service to find information about an incoming call.

#### Block incoming calls

When a phone receives an incoming call, the system first checks the person’s block list to determine whether to block the call. If the phone number isn’t on a user- or system-defined block list, the system then checks your app’s Call Directory app extension to find a matching blocked number. This is useful for apps that maintain a database of known solicitors, or allow someone to block any numbers that match a set of criteria.

To block incoming calls for a particular phone number, you use the addBlockingEntry(withNextSequentialPhoneNumber:) method in the implementation of beginRequest(with:).

Note

You can specify that your Call Directory app extension adds identification and blocks phone numbers in its implementation of beginRequest(with:).

- Swift
- Objective-C

```
class CustomCallDirectoryProvider: CXCallDirectoryProvider {
    override func beginRequest(with context: CXCallDirectoryExtensionContext) {
        let blockedPhoneNumbers: [CXCallDirectoryPhoneNumber] = [ … ]
        for phoneNumber in blockedPhoneNumbers.sorted(by: 

```
```

### Handle audio session interruptions

Like other audio apps, VoIP apps need to handle audio session interruptions. Interruptions may occur for several reasons, including a person accepting another call or closing the Smart Folio of their iPad. In these situations, an interruption notification contains the reason for the interruption and allows your app to correctly terminate the call, if necessary. For more information, see Handling audio interruptions.

## See Also

### Caller ID

class CXCallDirectoryProvider

The principal object for a Call Directory app extension for a host app.

class CXCallDirectoryExtensionContext

A programmatic interface for adding identification and blocking entries to a Call Directory app extension.

protocol CXCallDirectoryExtensionContextDelegate

A collection of methods a Call Directory extension context object calls when a request fails.

class CXCallDirectoryManager

The programmatic interface to an object that manages a Call Directory app extension.

