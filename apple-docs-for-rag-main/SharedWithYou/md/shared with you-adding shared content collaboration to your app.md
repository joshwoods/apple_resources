

- Shared With You
-  Adding shared content collaboration to your app 

Article

# Adding shared content collaboration to your app

Manage shared content collaboration in your app using CloudKit and iCloud Drive.

## Overview

Your app can create collaborations and share content in a Messages conversation by leveraging CloudKit and iCloud Drive to create and store content on the server. Collaborators add a document to conversations by sharing content using Messages. The system displays collaboration activity in Messages conversations and in active FaceTime calls.

This collaboration process builds on existing technologies, like drag and drop and the system share sheet. If your app doesn’t use iCloud for shared content, the Shared With You framework provides an SWCollaborationMetadata object wrapped in NSItemProvider to implement a custom collaboration infrastructure.

### Create a collaboration object

If your app is sharing a file URL using iCloud Drive, that URL is your collaboration object. To manage a CloudKit collaboration, your app uses NSItemProvider to register a CKShare container and create a collaboration object. The system transports your app’s data to other processes using the `CKShare` container.

Your app gives an existing `CKShare` to the collaboration object or provides a preparation handler to create a `CKShare` when collaboration starts. In the example below, your app starts a new collaboration and creates the `CKShare` container.

```
// Create a new collaboration object.

let itemProvider = NSItemProvider()
itemProvider.registerCKShare(container: container, allowedSharingOptions: CKAllowedSharingOptions.standard, preparationHandler: {
    // Create your share and save to the server or throw an error.
    return savedShare
})
```

For an existing collaboration, your app retrieves the existing collaboration object from the server.

```
// Retrieve an existing collaboration object.

let itemProvider = NSItemProvider()
itemProvider.registerCKShare(share, container: container, allowedSharingOptions: CKAllowedSharingOptions.standard)
```

### Present collaboration controls

A collaborator can modify the share options from the share sheet. To add the collaboration controls to the header of a share sheet, your app provides the collaboration object that it created or retrieved from the server.

```
// Present a share sheet in iOS.

let activityViewController = UIActivityViewController(activityItems: [collaborationObject], applicationActivities: nil)

presentingViewController.present(activityViewController, animated: true)
```

In macOS, a share popover offers similar options to the iOS share sheet.

```
// Present a share popover in macOS.

let sharingServicePicker = NSSharingServicePicker(items: [collaborationObject])

sharingServicePicker.show(relativeTo: view.bounds, of: view, preferredEdge: .minY)
```

### Provide a title and image for the collaboration header

If your app provides a file as shared data, the system automatically populates a title and image for the collaboration header in the share sheet. Otherwise, if your app uses CloudKit data as shared content, or if you’d like to override the default title and image, you can provide a title and image for the collaboration header.

In iOS, create a UIActivityItemsConfiguration with a title and image that your app passes to a UIActivityViewController.

```
// Provide CloudKit metadata in iOS.

let configuration = UIActivityItemsConfiguration(itemProviders: [collaborationItemProvider])
configuration.perItemMetadataProvider = { (_, key) in
    switch key {
    case .linkPresentationMetadata:
        // Create LPLinkMetadata with the title and imageProvider.
        return metadata
    default:
        return nil
    }
}

let activityViewController = UIActivityViewController(activityItemsConfiguration: configuration)
```

In macOS, create an NSPreviewRepresentingActivityItem with a title, image, and icon that your app passes to an NSSharingServicePicker. The image represents the shared content, and the icon represents the source of the shared content.

```
// Provide CloudKit metadata in macOS.

let title = “Shared Item”
let image = NSImage(contentsOfFile: “Shared_Item_Preview_Image.png”)
let icon = NSImage(contentsOfFile: “App_Icon.png”)

let previewRepresentingItem = NSPreviewRepresentingActivityItem(item: collaborationItemProvider, title: title, image: image, icon: icon)

let picker = NSSharingServicePicker(items: [previewRepresentingItem])
```

### Create a SwiftUI transferable object for collaboration through ShareLink

In SwiftUI, use ShareLink to support collaboration mode in the share sheet. The object your app shares must adopt Transferable, a protocol for sharing and data transfer.

In the example below, a structure provides a CKShareTransferRepresentation by either returning an existing CKShare or creating a new one.

```
// Create a SwiftUI Transferable object.

struct Note: Transferable {
    var share: CKShare?
    func saveCKShareToServer() async throws -> CKShare { … }

    static var transferRepresentation: some TransferRepresentation {
        CKShareTransferRepresentation { note in
            if let share = note.share {
                return .existing(share, container: container, options: options)
            } else {
                return .prepareShare(container: container, options: options) {
                    return try await note.saveCKShareToServer()
                }
            }
        }
    }
}
```

If your app is sharing a file URL using iCloud Drive, that URL is the `Transferable` object shared through `ShareLink`.

Once your app creates a `Transferable` object, pass it to `ShareLink`. When your app shares a URL or string, the system automatically creates a preview. Optionally, your app can include a SharePreview object, which the system uses to display the title and image for the preview.

```
// Adopt a SwiftUI ShareLink.

struct ContentView: View {
    // SharedPhoto() returns an object that conforms to the Transferable protocol.
    @State let photo = SharedPhoto()

    var body: some View {
        ShareLink(item: photo, preview: SharePreview(photo.title, image: photo.image))
    }
}
```

### Initialize the collaboration view

A collaborator accesses the SWCollaborationView using an icon in the navigation bar. This icon shows the app that manages the shared content and the number of collaborators associated with the collaboration.

The system handles the layout and formatting of the collaboration view. Your app is responsible for providing the `itemProvider(_:)` and the activeParticipantCount. The NSItemProvider contains the CKShare for CloudKit-based apps, the file URL for iCloud Drive-based apps, or the `/SharedWithYouCore/SWCollaborationMetadata/Representation` for custom collaboration infrastructures.

```
// Initialize the collaboration view.

let collaborationView = SWCollaborationView(itemProvider: itemProvider)

collaborationView.activeParticipantCount = myModel.activePeople.count
```

To add a completely customized view on the collaboration view, your app creates a view and assigns it to the `contentView`.

```
collaborationView.contentView = MyView(model: myModel)
```

For CloudKit and iCloud Drive adopters, the collaboration view includes a manage button. The button brings up the manage user interface, where collaborators can add and remove participants or change the share settings. Your app can also assign a custom title to the manageButtonTitle. The title defaults to “Manage Share” if your app doesn’t customize it.

```
collaborationView.manageButtonTitle = "Custom Manage Button"
```

If your app uses a custom collaboration infrastructure, you must provide your own manage button.

### Observe when a server saves a share

Since your app needs to manage active content sharing, it’s critical to know when a share starts or stops. If your app uses CloudKit or iCloud Drive, Shared with You provides a CKSystemSharingUIObserver protocol that your app uses to observe and handle updates to collaborations.

First, your app passes a CKContainer to `CKSystemSharingUIObserver` to create an observer.

```
let observer = CKSystemSharingUIObserver(container: container)
```

Then use the systemSharingUIDidSaveShareBlock in that observer to capture and react to the result of the server-side save of the share.

```
observer.systemSharingUIDidSaveShareBlock = { _, result in
    switch result {
    case .success(let share):
        // Handle the successful save of a share.
    case .failure(let error):
        // Handle the error for an unsuccessful save.
    }
}
```

Use the systemSharingUIDidStopSharingBlock in that same observer to handle when a share stops.

```
observer.systemSharingUIDidStopSharingBlock = { _, result in
    switch result {
    case .success(let share):
        // Handle the successful share deletion.
    case .failure(let error):
        // Handle the error when a deletion fails.
    }
}
```

### Post notices for shared content collaboration

Your app can post notices to summarize updates to a collaboration. These notices appear at the top of the related Messages thread. These updates include changes to the shared content, new mentions, server-side changes, and updates to the collaborators.

To post a notice, retrieve the SWCollaborationHighlight and use it to create an SWHighlightEvent that matches the type of update.

Use SWHighlightChangeEvent to post a notice about content updates or comments. Use SWHighlightCenter to retrieve a collaboration highlight with the URL of the CKShare your app used to initiate the collaboration.

```
// Retrieve the collaboration highlight from the highlight center.

let highlightCenter: SWHighlightCenter = self.highlightCenter

let highlight = try highlightCenter.collaborationHighlight(forURL: ckShareURL, error: &error)
```

Next, create an `SWHighlightChangeEvent` instance. The initializer takes an SWHighlight object and an SWHighlightChangeEventTrigger value. In this case, the app sets the trigger type to SWHighlightChangeEventTrigger.edit. Lastly, post the notice for that event to the highlight center.

```
// Post a change event notice.

let editEvent = SWHighlightChangeEvent(highlight: highlight, trigger: .edit)

highlightCenter.postNotice(for: editEvent)
```

### Post a persistence event notice

Use the SWHighlightPersistenceEvent to post a notice when your app moves, renames, or deletes content on the server. In the example below, the SWHighlightPersistenceEventTrigger.renamed trigger type signifies the document name has changed.

```
// Post a persistence event notice that shows your app renamed a document.

let renamedEvent = SWHighlightPersistenceEvent(highlight: highlight, trigger: .renamed)

highlightCenter.postNotice(for: renamedEvent)
```

### Post a membership event notice

When your app alters the membership for a collaboration and triggers a membership event, the system posts an update to the collaborators.

After your app retrieves the highlight, create the membership event by passing in the retrieved highlight. Use either SWHighlightMembershipEventTrigger.addedCollaborator or SWHighlightMembershipEventTrigger.removedCollaborator as the trigger for the SWHighlightMembershipEvent.

```
// Post a membership event notice that shows your app added a collaborator.

let membershipEvent = SWHighlightMembershipEvent(highlight: highlight, trigger: .addedCollaborator)

highlightCenter.postNotice(for: membershipEvent)
```

If the membership of a Messages group changes, Shared with You keeps collaborators on your shared documents in sync. For CloudKit and iCloud Drive, your app doesn’t have to do anything.

When a person adds someone new to a Messages conversation for a collaboration, the system prompts the document owner in Messages to add them to the share. When a person removes someone from a Messages conversation, the system prompts the document owner in Messages to remove them from the share.

## See Also

### Collaboration

Adding custom collaboration to your app

Integrate your custom collaboration app with Messages.

Collaboration views

Create and customize a collaboration view to manage the shared content actions.

