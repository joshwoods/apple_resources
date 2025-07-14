

- SwiftUI
- View fundamentals
- View
-  Presentation modifiers 

API Collection

# Presentation modifiers

Define additional views for the view to present under specified conditions.

## Overview

Use presentation modifiers to show different kinds of modal presentations, like alerts, popovers, sheets, and confirmation dialogs.

Because SwiftUI is a declarative framework, you don’t call a method at the moment you want to present the modal. Rather, you define how the presentation looks and the condition under which SwiftUI should present it. SwiftUI detects when the condition changes and makes the presentation for you. Because you provide a Binding to the condition that initiates the presentation, SwiftUI can reset the underlying value when the user dismisses the presentation.

For more information about how to use these modifiers, see Modal presentations.

## Topics

### Alerts

func alert(_:isPresented:actions:)

Presents an alert when a given condition is true, using a text view for the title.

func alert(_:isPresented:presenting:actions:)

Presents an alert using the given data to produce the alert’s content and a text view as a title.

func alert&lt;E, A>(isPresented: Binding&lt;Bool>, error: E?, actions: () -> A) -> some View

Presents an alert when an error is present.

### Alerts with a message

func alert(_:isPresented:actions:message:)

Presents an alert with a message when a given condition is true using a text view as a title.

func alert(_:isPresented:presenting:actions:message:)

Presents an alert with a message using the given data to produce the alert’s content and a text view for a title.

func alert&lt;E, A, M>(isPresented: Binding&lt;Bool>, error: E?, actions: (E) -> A, message: (E) -> M) -> some View

Presents an alert with a message when an error is present.

### Confirmation dialogs

func confirmationDialog(_:isPresented:titleVisibility:actions:)

Presents a confirmation dialog when a given condition is true, using a text view for the title.

func confirmationDialog(_:isPresented:titleVisibility:presenting:actions:)

Presents a confirmation dialog using data to produce the dialog’s content and a text view for the title.

func dismissalConfirmationDialog(_:shouldPresent:actions:)

Presents a confirmation dialog when a dismiss action has been triggered.

### Confirmation dialogs with a message

func confirmationDialog(_:isPresented:titleVisibility:actions:message:)

Presents a confirmation dialog with a message when a given condition is true, using a text view for the title.

func confirmationDialog(_:isPresented:titleVisibility:presenting:actions:message:)

Presents a confirmation dialog with a message using data to produce the dialog’s content and a text view for the message.

func dismissalConfirmationDialog(_:shouldPresent:actions:message:)

Presents a confirmation dialog when a dismiss action has been triggered.

### Dialog configuration

func dialogIcon(Image?) -> some View

Configures the icon used by dialogs within this view.

func dialogSeverity(DialogSeverity) -> some View

func dialogSuppressionToggle(isSuppressed: Binding&lt;Bool>) -> some View

Enables user suppression of dialogs and alerts presented within `self`, with a default suppression message on macOS. Unused on other platforms.

func dialogSuppressionToggle(_:isSuppressed:)

Enables user suppression of dialogs and alerts presented within `self`, with a custom suppression message on macOS. Unused on other platforms.

### Sheets

func sheet&lt;Content>(isPresented: Binding&lt;Bool>, onDismiss: (() -> Void)?, content: () -> Content) -> some View

Presents a sheet when a binding to a Boolean value that you provide is true.

func sheet&lt;Item, Content>(item: Binding&lt;Item?>, onDismiss: (() -> Void)?, content: (Item) -> Content) -> some View

Presents a sheet using the given item as a data source for the sheet’s content.

func fullScreenCover&lt;Content>(isPresented: Binding&lt;Bool>, onDismiss: (() -> Void)?, content: () -> Content) -> some View

Presents a modal view that covers as much of the screen as possible when binding to a Boolean value you provide is true.

func fullScreenCover&lt;Item, Content>(item: Binding&lt;Item?>, onDismiss: (() -> Void)?, content: (Item) -> Content) -> some View

Presents a modal view that covers as much of the screen as possible using the binding you provide as a data source for the sheet’s content.

### Popovers

func popover&lt;Item, Content>(item: Binding&lt;Item?>, attachmentAnchor: PopoverAttachmentAnchor, arrowEdge: Edge?, content: (Item) -> Content) -> some View

Presents a popover using the given item as a data source for the popover’s content.

func popover&lt;Content>(isPresented: Binding&lt;Bool>, attachmentAnchor: PopoverAttachmentAnchor, arrowEdge: Edge?, content: () -> Content) -> some View

Presents a popover when a given condition is true.

### Sheet and popover configuration

func interactiveDismissDisabled(Bool) -> some View

Conditionally prevents interactive dismissal of presentations like popovers, sheets, and inspectors.

func presentationDetents(Set&lt;PresentationDetent>) -> some View

Sets the available detents for the enclosing sheet.

func presentationDetents(Set&lt;PresentationDetent>, selection: Binding&lt;PresentationDetent>) -> some View

Sets the available detents for the enclosing sheet, giving you programmatic control of the currently selected detent.

func presentationDragIndicator(Visibility) -> some View

Sets the visibility of the drag indicator on top of a sheet.

func presentationBackground&lt;S>(S) -> some View

Sets the presentation background of the enclosing sheet using a shape style.

func presentationBackground&lt;V>(alignment: Alignment, content: () -> V) -> some View

Sets the presentation background of the enclosing sheet to a custom view.

func presentationBackgroundInteraction(PresentationBackgroundInteraction) -> some View

Controls whether people can interact with the view behind a presentation.

func presentationCompactAdaptation(horizontal: PresentationAdaptation, vertical: PresentationAdaptation) -> some View

Specifies how to adapt a presentation to horizontally and vertically compact size classes.

func presentationCompactAdaptation(PresentationAdaptation) -> some View

Specifies how to adapt a presentation to compact size classes.

func presentationContentInteraction(PresentationContentInteraction) -> some View

Configures the behavior of swipe gestures on a presentation.

func presentationCornerRadius(CGFloat?) -> some View

Requests that the presentation have a specific corner radius.

func presentationSizing(some PresentationSizing) -> some View

Sets the sizing of the containing presentation.

### File exporter

func fileExporter(isPresented:document:contentType:defaultFilename:onCompletion:)

Presents a system interface for exporting a document that’s stored in a value type, like a structure, to a file on disk.

func fileExporter(isPresented:documents:contentType:onCompletion:)

Presents a system interface for exporting a collection of value type documents to files on disk.

func fileExporter(isPresented:document:contentTypes:defaultFilename:onCompletion:onCancellation:)

Presents a system interface for allowing the user to export a `FileDocument` to a file on disk.

func fileExporter(isPresented:documents:contentTypes:onCompletion:onCancellation:)

Presents a system dialog for allowing the user to export a collection of documents that conform to `FileDocument` to files on disk.

func fileExporter&lt;T>(isPresented: Binding&lt;Bool>, item: T?, contentTypes: [UTType], defaultFilename: String?, onCompletion: (Result&lt;URL, any Error>) -> Void, onCancellation: () -> Void) -> some View

Presents a system interface allowing the user to export a `Transferable` item to file on disk.

func fileExporter&lt;C, T>(isPresented: Binding&lt;Bool>, items: C, contentTypes: [UTType], onCompletion: (Result&lt;[URL], any Error>) -> Void, onCancellation: () -> Void) -> some View

Presents a system interface allowing the user to export a collection of items to files on disk.

func fileExporterFilenameLabel(_:)

On macOS, configures the `fileExporter` with a text to use as a label for the file name field.

### File importer

func fileImporter(isPresented: Binding&lt;Bool>, allowedContentTypes: [UTType], allowsMultipleSelection: Bool, onCompletion: (Result&lt;[URL], any Error>) -> Void) -> some View

Presents a system interface for allowing the user to import multiple files.

func fileImporter(isPresented: Binding&lt;Bool>, allowedContentTypes: [UTType], onCompletion: (Result&lt;URL, any Error>) -> Void) -> some View

Presents a system interface for allowing the user to import an existing file.

func fileImporter(isPresented: Binding&lt;Bool>, allowedContentTypes: [UTType], allowsMultipleSelection: Bool, onCompletion: (Result&lt;[URL], any Error>) -> Void, onCancellation: () -> Void) -> some View

Presents a system dialog for allowing the user to import multiple files.

### File mover

func fileMover(isPresented: Binding&lt;Bool>, file: URL?, onCompletion: (Result&lt;URL, any Error>) -> Void) -> some View

Presents a system interface for allowing the user to move an existing file to a new location.

func fileMover&lt;C>(isPresented: Binding&lt;Bool>, files: C, onCompletion: (Result&lt;[URL], any Error>) -> Void) -> some View

Presents a system interface for allowing the user to move a collection of existing files to a new location.

func fileMover(isPresented: Binding&lt;Bool>, file: URL?, onCompletion: (Result&lt;URL, any Error>) -> Void, onCancellation: () -> Void) -> some View

Presents a system dialog for allowing the user to move an existing file to a new location.

func fileMover&lt;C>(isPresented: Binding&lt;Bool>, files: C, onCompletion: (Result&lt;[URL], any Error>) -> Void, onCancellation: () -> Void) -> some View

Presents a system dialog for allowing the user to move a collection of existing files to a new location.

### File dialog configuration

func fileDialogBrowserOptions(FileDialogBrowserOptions) -> some View

On macOS, configures the `fileExporter`, `fileImporter`, or `fileMover` to provide a refined URL search experience: include or exclude hidden files, allow searching by tag, etc.

func fileDialogConfirmationLabel(_:)

On macOS, configures the the `fileExporter`, `fileImporter`, or `fileMover` with custom text as a confirmation button label.

func fileDialogCustomizationID(String) -> some View

On macOS, configures the `fileExporter`, `fileImporter`, or `fileMover` to persist and restore the file dialog configuration.

func fileDialogDefaultDirectory(URL?) -> some View

Configures the `fileExporter`, `fileImporter`, or `fileMover` to open with the specified default directory.

func fileDialogImportsUnresolvedAliases(Bool) -> some View

On macOS, configures the `fileExporter`, `fileImporter`, or `fileMover` behavior when a user chooses an alias.

func fileDialogMessage(_:)

On macOS, configures the the `fileExporter`, `fileImporter`, or `fileMover` with a custom text that is presented to the user, similar to a title.

func fileDialogURLEnabled(Predicate&lt;URL>) -> some View

On macOS, configures the the `fileImporter` or `fileMover` to conditionally disable presented URLs.

### Inspectors

func inspector&lt;V>(isPresented: Binding&lt;Bool>, content: () -> V) -> some View

Inserts an inspector at the applied position in the view hierarchy.

func inspectorColumnWidth(CGFloat) -> some View

Sets a fixed, preferred width for the inspector containing this view when presented as a trailing column.

func inspectorColumnWidth(min: CGFloat?, ideal: CGFloat, max: CGFloat?) -> some View

Sets a flexible, preferred width for the inspector in a trailing-column presentation.

### Quick look previews

func quickLookPreview(Binding&lt;URL?>) -> some View

Presents a Quick Look preview of the contents of a single URL.

func quickLookPreview&lt;Items>(Binding&lt;Items.Element?>, in: Items) -> some View

Presents a Quick Look preview of the URLs you provide.

### Family Sharing

func familyActivityPicker(isPresented: Binding&lt;Bool>, selection: Binding&lt;FamilyActivitySelection>) -> some View

Presents an activity picker view as a sheet.

func familyActivityPicker(headerText: String?, footerText: String?, isPresented: Binding&lt;Bool>, selection: Binding&lt;FamilyActivitySelection>) -> some View

Presents an activity picker view as a sheet.

### Live Activities

func activitySystemActionForegroundColor(Color?) -> some View

The text color for the auxiliary action button that the system shows next to a Live Activity on the Lock Screen.

func activityBackgroundTint(Color?) -> some View

Sets the tint color for the background of a Live Activity that appears on the Lock Screen.

### Apple Music

func musicSubscriptionOffer(isPresented: Binding&lt;Bool>, options: MusicSubscriptionOffer.Options, onLoadCompletion: ((any Error)?) -> Void) -> some View

Initiates the process of presenting a sheet with subscription offers for Apple Music when the `isPresented` binding is `true`.

### StoreKit

func appStoreOverlay(isPresented: Binding&lt;Bool>, configuration: () -> SKOverlay.Configuration) -> some View

Presents a StoreKit overlay when a given condition is true.

func manageSubscriptionsSheet(isPresented: Binding&lt;Bool>) -> some View

func refundRequestSheet(for: Transaction.ID, isPresented: Binding&lt;Bool>, onDismiss: ((Result&lt;Transaction.RefundRequestStatus, Transaction.RefundRequestError>) -> ())?) -> some View

Display the refund request sheet for the given transaction.

func offerCodeRedemption(isPresented: Binding&lt;Bool>, onCompletion: (Result&lt;Void, any Error>) -> Void) -> some View

Presents a sheet that enables users to redeem subscription offer codes that you configure in App Store Connect.

### PhotoKit

func photosPicker(isPresented: Binding&lt;Bool>, selection: Binding&lt;PhotosPickerItem?>, matching: PHPickerFilter?, preferredItemEncoding: PhotosPickerItem.EncodingDisambiguationPolicy) -> some View

Presents a Photos picker that selects a `PhotosPickerItem`.

func photosPicker(isPresented: Binding&lt;Bool>, selection: Binding&lt;PhotosPickerItem?>, matching: PHPickerFilter?, preferredItemEncoding: PhotosPickerItem.EncodingDisambiguationPolicy, photoLibrary: PHPhotoLibrary) -> some View

Presents a Photos picker that selects a `PhotosPickerItem` from a given photo library.

func photosPicker(isPresented: Binding&lt;Bool>, selection: Binding&lt;[PhotosPickerItem]>, maxSelectionCount: Int?, selectionBehavior: PhotosPickerSelectionBehavior, matching: PHPickerFilter?, preferredItemEncoding: PhotosPickerItem.EncodingDisambiguationPolicy) -> some View

Presents a Photos picker that selects a collection of `PhotosPickerItem`.

func photosPicker(isPresented: Binding&lt;Bool>, selection: Binding&lt;[PhotosPickerItem]>, maxSelectionCount: Int?, selectionBehavior: PhotosPickerSelectionBehavior, matching: PHPickerFilter?, preferredItemEncoding: PhotosPickerItem.EncodingDisambiguationPolicy, photoLibrary: PHPhotoLibrary) -> some View

Presents a Photos picker that selects a collection of `PhotosPickerItem` from a given photo library.

func photosPickerAccessoryVisibility(Visibility, edges: Edge.Set) -> some View

Sets the accessory visibility of the Photos picker. Accessories include anything between the content and the edge, like the navigation bar or the sidebar.

func photosPickerDisabledCapabilities(PHPickerCapabilities) -> some View

Disables capabilities of the Photos picker.

func photosPickerStyle(PhotosPickerStyle) -> some View

Sets the mode of the Photos picker.

## See Also

### Providing interactivity

Input and event modifiers

Supply actions for a view to perform in response to user input and system events.

Search modifiers

Enable people to search for content in your app.

State modifiers

Access storage and provide child views with configuration data.

