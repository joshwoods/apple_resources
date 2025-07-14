

- Shared With You
-  Adding custom collaboration to your app 

Article

# Adding custom collaboration to your app

Integrate your custom collaboration app with Messages.

## Overview

If your app uses iCloud to store shared content, you can use the steps in Adding shared content collaboration to your app to add collaboration. To share content without using iCloud, the Shared with You framework provides an SWCollaborationMetadata object wrapped in NSItemProvider to implement a custom collaboration infrastructure.

Before you can use this collaboration infrastructure, your app needs to support universal links to share content with other apps. For more details about implementing universal links, see Making your app content shareable.

Related sessions from WWDC22

Session 10093: Integrate your custom collaboration app with Messages

### Create the metadata object

When a user decides to share a collaboration from your app through the Messages app, you first create metadata to represent the content. The metadata includes share options the user can configure prior to sending the message, and many other properties you can customize. Next, you provide that metadata to the share sheet, or to drag and drop using the steps below in the “Present a collaboration view” section.

The string you pass to SWLocalCollaborationIdentifier doesn’t need to be unique across devices, it’s only for your app to use locally. Similarly, the system displays the initiator’s account handle and name that your app retrieves from personNameComponents(from:) locally so the collaborator can confirm their account.

```
```

After your app sets the identifier and initiator for the metadata, configure SWCollaborationShareOptions. Share options are the settings a person configures on the collaboration in Messages or the share sheet. Options represent individual switches, or mutually exclusive values for a setting. Options have a title and an identifier, and are either in a selected or an unselected state.

There are two classes to represent a group of options: SWCollaborationOptionsGroup and SWCollaborationOptionsPickerGroup. Use `SWCollaborationOptionsGroup` to represent a collection of switches, and use `SWCollaborationOptionsPickerGroup` to represent mutually exclusive values for a setting.

In the example below, a person can choose either the “Can make changes” or the “Read only” option. The collaborator can choose “Allow mentions” and the “Allow comments” options independent of each other. The app then passes both the option groups to `SWCollaborationShareOptions` to initialize the defaultShareOptions.

```
```

### Present a collaboration view

If your app uses SwiftUI, SWCollaborationMetadata is compatible with the Transferable protocol and the ShareLink view. In the example below, the app defines a `Transferable` model object and creates a ProxyRepresentation to return a collaboration metadata instance. Then, the app passes that model object to a `ShareLink` instance in the view.

```
```

It’s good practice to register multiple representations of the content to support sharing through as many channels as possible. For example, Messages automatically offers an option to send the content as a copy if you provide a file representation.

For UIKit and AppKit apps, use NSItemProvider to support content sharing. `SWCollaborationMetadata` conforms to the NSItemProviderReading and NSItemProviderWriting protocols, so you can register a metadata instance with an item provider to support collaboration. Use `NSItemProvider` with UIActivityViewController and UIDragItem in iOS and iPadOS, and NSSharingServicePicker in macOS.

In the example code below, the app registers the collaboration metadata in an `NSItemProvider` instance. Then the app creates a UIActivityItemsConfiguration object with the item provider object and passes that to the `UIActivityViewController`. Finally, the app presents the share sheet.

```
```

To support drag and drop in iOS, initialize `NSItemProvider` and register the metadata the same way as in the previous code example, then create a UIDragItem with the item provider.

```
```

The API is similar in macOS for the sharing popover. Use the item provider to initialize an NSSharingServicePicker object and show the picker relative to a target view.

```
```

To support drag and drop in macOS, use NSPasteboardItem instead of `NSItemProvider`. Assign the collaboration metadata to collaborationMetadata on a new `NSPasteboardItem` instance.

```
```

The system stages a draft of your collaborative content in Messages. After a person taps the Send button, the system coordinates with your app to create the share.

### Prepare the collaboration coordinator

`SWCollaborationCoordinator` is a singleton, meaning there’s a global shared instance that your app uses to respond to action requests. Your app defines an action handler that conforms to the SWCollaborationActionHandler protocol. Because the collaboration coordinator runs in the background and can send requests for actions to your app at any time, define your action handler early in the launch process. The app in the example below registers the handler in the application(_:didFinishLaunchingWithOptions:) method:

```
```

Your action handler is responsible for responding to SWAction requests from the system. An `SWAction` represents work your app needs to handle during a collaboration. Your app calls fulfill() after it completes a request. If your app can’t complete an action, it responds with fail(). It’s important to respond to `SWAction` requests quickly to avoid a system timeout.

The example code below retrieves the localIdentifier and userSelectedShareOptions from the SWCollaborationMetadata in the action. The `APIRequest` object in this example is the API for processing collaboration requests on a web server.

```
```

If the SWStartCollaborationAction is successful, the system sends your app a second action to update the collaboration participants. Before you can add or remove participants, your app needs to have a way to verify participants.

### Verify participant access

The SWUpdateCollaborationParticipantsAction contains the cryptographic identities for the participants. The system derives the identities from the collaboration identifier that `SWStartCollaborationAction` provides. Your shared content server is responsible for identity storage and verification of recipient devices.

To verify a participant, use the SWPerson.Identity rootHash property. A root hash is a secure value your app sends to your server to uniquely identify a participant on their devices. To perform a verification, your server needs to compute a root hash.

When the system sends a collaboration message for a participant, it actually sends individual messages to each device for that participant. The Messages app identifies each device using a cryptographic public key. Because the goal is to allow access only on this participant’s set of devices, the system derives the root hash from the set of public keys registered to each recipient.

The root hash is the root node of a data structure called a *Merkle tree*. A Merkle tree is a binary tree that the system builds by performing a sequence of hashing operations. To derive an identity for the participant based on their public keys, the system uses the keys as the *leaves* of this tree. The hashing algorithm that the system uses in the Merkle tree ensures that the system can only compute the root node from that set of keys.

In the example below, the user has three devices and three public keys. The keys are unique for each collaboration identifier that your app provides, using a process called key diversification. To prevent tracking the number of devices registered to a user, the system pads the set with random keys up to a fixed size. Your server hashes the padded set of diversified keys to create the leaf nodes of the tree with a SHA-256 algorithm.

Your server then concatenates and hashes each pair of leaf nodes to derive their predecessor nodes. Repeat this process with the predecessor nodes until a single root node remains. This is the root hash that the system uses to uniquely represent this recipient’s identity across their devices.

The figure below shows that it’s possible to generate a root hash using a subset of the nodes from a complete Merkle tree. Your server can use the hashes H4, H7, and H11, along with the diversified public key P3, to reproduce the root hash in this tree. First, hash the public key to get the missing leaf node H3. Then use H3 and H4 to generate H8. Next, use the given H7 node with H8 to generate H10. Finally, use H10 and H11 to produce the root hash.

It’s important to note that you can prove the system uses the public key P3 to generate a given root hash, without needing to reconstruct the entire tree. The subset of nodes necessary to do this is a proof of inclusion. Verification begins when your app opens a universal link. To do this, you first need to check that the link is collaborative.

### Verify a collaboration link

SWCollaborationHighlight represents a collaborative link that your app retrieves from SWHighlightCenter. Use that collaboration highlight to generate the proof of inclusion. To represent a proof of inclusion, use SWPerson.IdentityProof. To perform verification, first generate this object along with a cryptographic signature to send to your server. Retrieve the proof using the getSignedIdentityProof(for:using:completionHandler:) method on `SWHighlightCenter`.

Use the signature to ensure that a bad actor can’t send the request to gain access to your collaboration. The data can be a challenge you request from your server, or a nonce that the device generates. The example below uses the challenge approach.

The system passes the URL, which is the universal link associated with a collaboration, to application(_:didFinishLaunchingWithOptions:). Use this URL to fetch the associated `SWCollaborationHighlight` from the `SWHighlightCenter`.

Request the challenge from the server, and pass the returned data to the `getSignedIdentityProof` method on `SWHighlightCenter`, along with the highlight. This method returns a signed identity proof that the app sends to the server for verification.

The app sends the proof to the server, along with the public key and the signed data. Your app signs the data using the Elliptic Curve Digital Signature Algorithm over the P-256 elliptic curve. Verify the signature on the data using the public key in the identity proof. You can do this with most common encryption libraries.

```
```

After you verify the signature, you can trust that the identity proof the system sends is from the device associated with that public key. Next, use the identity proof to recompute the root hash. A recursive algorithm works well with tree data structures, as in the code example below:

```
```

On the initial invocation, pass in the hash of the public key, the set of inclusion hashes, and the public key index. Next, remove the first inclusion hash. Check the public key index to see whether the key is on the left or the right of its sibling. Concatenate and hash the selected hashes in the correct order. Next, remove the consumed node in the `inclusionHashes` array, and pass the rest to a recursive call to this same function. The public key index then updates so that it’s ready for the next node in the tree.

With this simple function, you can quickly compute a root hash given an identity proof. The server can check that this generated root hash is in the list of root hashes the owner of the document uploads during sending. The hash is present in the list of known hashes, so the server can grant access to the document.

Next, sign some data and retrieve the proof of inclusion. Send the signed data and proof to your server. Verify the signature on the data. Using the proof of inclusion, generate the root hash. Finally, compare the root hash to the list of known identities associated with that content.

### Add a participant

The example below shows how to handle the update participants action. First, retrieve the collaboration identifier from the action’s metadata — this is the identifier you supply to the fulfill() method while handling `SWStartCollaborationAction`.

Next, use the action’s addedIdentities property to retrieve the participant data to store on your content server. Each identity has a rootHash property, which is the data you store on your server to validate participants during the collaboration process.

After you retrieve this data, create another server request to add the participants to the collaboration with the target identifier. Then, send the request to your server, and fulfill or fail the action. This time, the fulfill method doesn’t take any parameters. After you set up the collaboration, your app has everything it needs to grant immediate access to the recipients of the message.

```
```

### Remove a participant

To remove a participant, look up any account associated with a removed identity and revoke their access. If your app doesn’t have any associated accounts for this collaboration, delete the root hash from your database. The example code below uses the removedIdentities property on the action and passes it to a similar removal API request:

```
```

### Post a change event notice

When a participant makes changes to a collaboration, your app posts notices about those changes. The system displays those notices in Messages as a banner in the shared conversation. The banner includes a description of the changes, as well as the name of the person who makes each change.

Your app posts a change event for content updates or comments, and it posts a membership event when a participant joins or leaves. When a person mentions another person in a collaboration, post a mention event. Post a persistence event when a collaborator moves or deletes content. The example code below shows how to post a change event for an edit to a collaboration:

```
```

### Post a membership event notice

For participant changes, your app posts a membership event and passes either the SWHighlightMembershipEventTrigger.addedCollaborator or SWHighlightMembershipEventTrigger.removedCollaborator trigger type.

```
```

### Post a mention event notice

If your app supports user mentions, you can post a mention event. Initialize a person identity with the root hash of the mentioned user. Next, pass the mentioned identity to SWHighlightMentionEvent and post the mention event.

The system shows this notice only to the mentioned user in the Messages app.

```
```

### Post a persistence event notice

Your app posts the persistence event type when a participant moves, renames, or deletes content. In the example below, the app uses SWHighlightPersistenceEventTrigger.renamed to indicate that the participant changed the name of the content:

```
```

## See Also

### Collaboration

Adding shared content collaboration to your app

Manage shared content collaboration in your app using CloudKit and iCloud Drive.

Collaboration views

Create and customize a collaboration view to manage the shared content actions.

