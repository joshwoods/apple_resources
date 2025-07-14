

- Foundation
- NSNotification
-  NSNotification.Name 

Structure

# NSNotification.Name

A structure that defines the name of a notification.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct Name
```

## Topics

### AddressBook

static let abDatabaseChanged: NSNotification.Name

Posted when this process has changed the Address Book database.

static let abDatabaseChangedExternally: NSNotification.Name

Posted when a process other than the current one has changed the Address Book database.

static let ABPeoplePickerDisplayedPropertyDidChange: NSNotification.Name

Posted when the displayed property in the record list is changed.

static let ABPeoplePickerGroupSelectionDidChange: NSNotification.Name

Posted when the selection in the group list is changed.

static let ABPeoplePickerNameSelectionDidChange: NSNotification.Name

Posted when the selection in the name list is changed.

static let ABPeoplePickerValueSelectionDidChange: NSNotification.Name

Posted when the selection in a multivalue property is changed.

### AppKit

static let unsupportedAttributeAddedNotification: NSNotification.Name

class let didProcessEditingNotification: NSNotification.Name

A notification that posts after a text storage finishes processing edits.

class let willProcessEditingNotification: NSNotification.Name

A notification that posts before a text storage begins processing edits.

class let didChangeSelectionNotification: NSNotification.Name

Posted when the selected range of characters changes.

class let didChangeTypingAttributesNotification: NSNotification.Name

Posted when there is a change in the typing attributes within a text view.

class let willChangeNotifyingTextViewNotification: NSNotification.Name

Posted when a new text view is established as the text view that sends notifications.

class let didRemoveItemNotification: NSNotification.Name

Posted after an item is removed from a toolbar.

class let willAddItemNotification: NSNotification.Name

Posts before the toolbar adds a new item.

class let didUpdateTrackingAreasNotification: NSNotification.Name

Posted whenever a view recalculates its tracking areas.

class let didBecomeKeyNotification: NSNotification.Name

A notification that the window object became the key window.

class let didBecomeMainNotification: NSNotification.Name

A notification that the window object became the main window.

class let didChangeBackingPropertiesNotification: NSNotification.Name

A notification that the window object backing properties changed.

class let didChangeOcclusionStateNotification: NSNotification.Name

A notification that the window object’s occlusion state changed.

class let didChangeScreenNotification: NSNotification.Name

A notification that a portion of the window object’s frame moved onto or off of a screen.

class let didChangeScreenProfileNotification: NSNotification.Name

A notification that the screen containing the window changed.

class let didDeminiaturizeNotification: NSNotification.Name

A notification that the window is no longer minimized.

class let didEndLiveResizeNotification: NSNotification.Name

A notification that the user resized the window object.

class let didEndSheetNotification: NSNotification.Name

A notification that the window object closed an attached sheet.

class let didEnterFullScreenNotification: NSNotification.Name

A notification that the window entered full-screen mode.

class let didEnterVersionBrowserNotification: NSNotification.Name

A notification that the window object entered version browser mode.

class let didExitFullScreenNotification: NSNotification.Name

A notification that the window object exited full-screen mode.

class let didExitVersionBrowserNotification: NSNotification.Name

A notification that the window object exited version browser mode.

class let didExposeNotification: NSNotification.Name

A notification that a window exposed a portion of its nonretained content.

class let didMiniaturizeNotification: NSNotification.Name

A notification that the window object minimized.

class let didMoveNotification: NSNotification.Name

A notification that the window object moved.

class let didResignKeyNotification: NSNotification.Name

A notification that the window object resigned its status as key window.

class let didResignMainNotification: NSNotification.Name

A notification that the window object resigned its status as main window.

class let didResizeNotification: NSNotification.Name

A notification that the window object size changed.

class let didUpdateNotification: NSNotification.Name

A notification that the window object received an update message.

class let willBeginSheetNotification: NSNotification.Name

A notification that the window object is about to open a sheet.

class let willCloseNotification: NSNotification.Name

A notification that the window object is about to close.

class let willEnterFullScreenNotification: NSNotification.Name

A notification that the window will enter full-screen mode.

class let willEnterVersionBrowserNotification: NSNotification.Name

A notification that the window object will enter version browser mode.

class let willExitFullScreenNotification: NSNotification.Name

A notification that the window object will exit full-screen mode.

class let willExitVersionBrowserNotification: NSNotification.Name

A notification that the window object will exit version browser mode.

class let willMiniaturizeNotification: NSNotification.Name

A notification that the window object is about to minimize.

class let willMoveNotification: NSNotification.Name

A notification that the window object is about to move.

class let willStartLiveResizeNotification: NSNotification.Name

A notification that the user is about to resize the window.

class let accessibilityDisplayOptionsDidChangeNotification: NSNotification.Name

A notification that the workspace posts when any of the accessibility display options change.

class let activeSpaceDidChangeNotification: NSNotification.Name

A notification that the workspace posts when a Spaces change occurs.

class let didActivateApplicationNotification: NSNotification.Name

A notification that the workspace posts when the Finder is about to activate an app.

class let didChangeFileLabelsNotification: NSNotification.Name

A notification that the workspace posts when the Finder file labels or colors change.

class let didDeactivateApplicationNotification: NSNotification.Name

A notification that the workspace posts when the Finder deactivates an app.

class let didHideApplicationNotification: NSNotification.Name

A notification that the workspace posts when the Finder hides an app.

class let didLaunchApplicationNotification: NSNotification.Name

A notification that the workspace posts when a new app starts up.

class let didMountNotification: NSNotification.Name

A notification that the workspace posts when a new device mounts.

class let didPerformFileOperationNotification: NSNotification.Name

Posted when a file operation has been performed in the receiving app.

Deprecated

class let didRenameVolumeNotification: NSNotification.Name

A notification that the workspace posts when a volume changes its name or mount path.

class let didTerminateApplicationNotification: NSNotification.Name

A notification that the workspace posts when an app finishes executing.

class let didUnhideApplicationNotification: NSNotification.Name

A notification that the workspace posts when the Finder unhides an app.

class let didUnmountNotification: NSNotification.Name

A notification that the workspace posts when the Finder unmounts a device.

class let didWakeNotification: NSNotification.Name

A notification that the workspace posts when the device wakes from sleep.

class let screensDidSleepNotification: NSNotification.Name

A notification that the workspace posts when the device’s screen goes to sleep.

class let screensDidWakeNotification: NSNotification.Name

A notification that the workspace posts when the device’s screens wake.

class let sessionDidBecomeActiveNotification: NSNotification.Name

A notification that the workspace posts after a user session switches in.

class let sessionDidResignActiveNotification: NSNotification.Name

A notification that the workspace posts before a user session switches out.

class let willLaunchApplicationNotification: NSNotification.Name

A notification that the workspace posts when the Finder is about to launch an app.

class let willPowerOffNotification: NSNotification.Name

A notification that the workspace posts when the user requests a logout or powers off the device.

class let willSleepNotification: NSNotification.Name

A notification that the workspace posts before the device goes to sleep.

class let willUnmountNotification: NSNotification.Name

A notification that the workspace posts when the Finder is about to unmount a device.

class let didChangeNotification: NSNotification.Name

Posted whenever a color list changes.

class let selectionDidChangeNotification: NSNotification.Name

Posted after the pop-up list selection of the \`NSComboBox\` changes.

class let selectionIsChangingNotification: NSNotification.Name

Posted whenever the pop-up list selection of the \`NSComboBox\` is changing.

class let willDismissNotification: NSNotification.Name

Posted whenever the pop-up list of the \`NSComboBox\` is about to be dismissed.

class let willPopUpNotification: NSNotification.Name

Posted whenever the pop-up list of the \`NSComboBox\` is going to be displayed.

class let contextHelpModeDidActivateNotification: NSNotification.Name

Posted when the application enters context-sensitive help mode. This typically happens when the user holds down the Help key.

class let contextHelpModeDidDeactivateNotification: NSNotification.Name

Posted when the application exits context-sensitive help mode. This happens when the user clicks the mouse button while the cursor is anywhere on the screen after displaying a context-sensitive help topic.

class let textDidBeginEditingNotification: NSNotification.Name

Sent when a control with editable cells begins an edit session.

class let textDidChangeNotification: NSNotification.Name

Sent when the text in the receiving control changes.

class let textDidEndEditingNotification: NSNotification.Name

Sent when a control with editable cells ends an editing session.

class let currentControlTintDidChangeNotification: NSNotification.Name

Sent after the user changes control tint preference.

Deprecated

class let didCloseNotification: NSNotification.Name

Posted whenever the drawer is closed.

Deprecated

class let didOpenNotification: NSNotification.Name

Posted whenever the drawer is opened.

Deprecated

class let willCloseNotification: NSNotification.Name

Posted whenever the drawer is about to close.

Deprecated

class let willOpenNotification: NSNotification.Name

Posted whenever the drawer is about to open.

Deprecated

class let didChangeNotification: NSNotification.Name

Posted whenever a font collection is changed.

class let fontSetChangedNotification: NSNotification.Name

Posted after the currently-set font changes.

class let registryDidChangeNotification: NSNotification.Name

Posted whenever the image representation class registry changes.

class let didAddItemNotification: NSNotification.Name

Posted after a menu item is added to the menu.

class let didBeginTrackingNotification: NSNotification.Name

Posted when menu tracking begins.

class let didChangeItemNotification: NSNotification.Name

Posted after a menu item in the menu changes appearance.

class let didEndTrackingNotification: NSNotification.Name

Posted when menu tracking ends, even if no action is sent.

class let didRemoveItemNotification: NSNotification.Name

Posted after a menu item is removed from the menu.

class let didSendActionNotification: NSNotification.Name

Posted just after the application dispatches a menu item’s action method to the menu item’s target.

class let willSendActionNotification: NSNotification.Name

Posted just before the application dispatches a menu item’s action method to the menu item’s target.

class let columnDidMoveNotification: NSNotification.Name

Posted whenever a column is moved by user action in an \`NSOutlineView\` object.

class let columnDidResizeNotification: NSNotification.Name

Posted whenever a column is resized in an \`NSOutlineView\` object.

class let itemDidCollapseNotification: NSNotification.Name

Posted whenever an item is collapsed in an \`NSOutlineView\` object.

class let itemDidExpandNotification: NSNotification.Name

Posted whenever an item is expanded in an \`NSOutlineView\` object.

class let itemWillCollapseNotification: NSNotification.Name

Posted before an item is collapsed (after the user clicks the arrow but before the item is collapsed).

class let itemWillExpandNotification: NSNotification.Name

Posted before an item is expanded (after the user clicks the arrow but before the item is collapsed).

class let selectionDidChangeNotification: NSNotification.Name

Posted after the outline view’s selection changes.

class let selectionIsChangingNotification: NSNotification.Name

Posted as the outline view’s selection changes (while the mouse button is still down).

class let willPopUpNotification: NSNotification.Name

This notification is posted just before a pop-up menu is attached to its window frame.

class let willPopUpNotification: NSNotification.Name

Posted when an \`NSPopUpButton\` object receives a mouse-down event—that is, when the user is about to select an item from the menu.

class let didCloseNotification: NSNotification.Name

Sent after the popover has finished animating offscreen.

class let didShowNotification: NSNotification.Name

Sent after the popover has finished animating onscreen.

class let willCloseNotification: NSNotification.Name

Sent before the popover is closed.

class let willShowNotification: NSNotification.Name

Sent before the popover is shown.

class let preferredScrollerStyleDidChangeNotification: NSNotification.Name

Posted if the preferred scroller style changes.

class let rowsDidChangeNotification: NSNotification.Name

This notification is posted to the default notification center whenever the view’s rows change.

class let colorSpaceDidChangeNotification: NSNotification.Name

Posted when the color space of the screen has changed.

class let didEndLiveMagnifyNotification: NSNotification.Name

Posted at the end of a magnify gesture.

class let didEndLiveScrollNotification: NSNotification.Name

Posted on the main thread at the end of live scroll tracking.

class let didLiveScrollNotification: NSNotification.Name

Posted on the main thread after changing the clipview bounds origin due to a user-initiated event.

class let willStartLiveMagnifyNotification: NSNotification.Name

Posted at the beginning of a magnify gesture.

class let willStartLiveScrollNotification: NSNotification.Name

Posted on the main thread at the beginning of user-initiated live scroll tracking (gesture scroll or scroller tracking, for example, thumb dragging).

class let didChangeAutomaticCapitalizationNotification: NSNotification.Name

class let didChangeAutomaticDashSubstitutionNotification: NSNotification.Name

class let didChangeAutomaticPeriodSubstitutionNotification: NSNotification.Name

class let didChangeAutomaticQuoteSubstitutionNotification: NSNotification.Name

class let didChangeAutomaticSpellingCorrectionNotification: NSNotification.Name

This notification is posted when the spell checker did change text using automatic spell checking correction. The are posted to the application’s default notification center.

class let didChangeAutomaticTextReplacementNotification: NSNotification.Name

Posted when the spell checker changed text using automatic text replacement. This notification is posted to the app’s default notification center.

class let didResizeSubviewsNotification: NSNotification.Name

A notification that posts after a change to the size of some or all subviews of a split view.

class let willResizeSubviewsNotification: NSNotification.Name

A notification that posts before a change to the size of some or all subviews of a split view.

class let systemColorsDidChangeNotification: NSNotification.Name

Sent when the system colors have changed, such as through a system control panel interface.

class let columnDidMoveNotification: NSNotification.Name

Posted whenever a column is moved by user action in an \`NSTableView\` object.

class let columnDidResizeNotification: NSNotification.Name

Posted whenever a column is resized in an \`NSTableView\` object.

class let selectionDidChangeNotification: NSNotification.Name

Posted after an \`NSTableView\` object’s selection changes.

class let selectionIsChangingNotification: NSNotification.Name

Posted as an \`NSTableView\` object’s selection changes (while the mouse button is still down).

class let selectedAlternativeStringNotification: NSNotification.Name

Posted when the user selects an alternate string.

class let didBeginEditingNotification: NSNotification.Name

Posted when an \`NSText\` object begins any operation that changes characters or formatting attributes.

class let didChangeNotification: NSNotification.Name

Posted after an \`NSText\` object performs any operation that changes characters or formatting attributes.

class let didEndEditingNotification: NSNotification.Name

Posted when focus leaves an \`NSText\` object, whether or not any operation has changed characters or formatting attributes.

class let keyboardSelectionDidChangeNotification: NSNotification.Name

Posted after the selected text input source changes.

class let didChangeAutomaticTextCompletionNotification: NSNotification.Name

class let didBecomeActiveNotification: NSNotification.Name

Posted immediately after the app becomes active.

class let didChangeOcclusionStateNotification: NSNotification.Name

Posted when the app’s occlusion state changes.

class let didChangeScreenParametersNotification: NSNotification.Name

Posted when the configuration of the displays attached to the computer is changed.

class let didFinishRestoringWindowsNotification: NSNotification.Name

Posted when the app has finished restoring windows.

class let didResignActiveNotification: NSNotification.Name

Posted immediately after the app gives up its active status to another app.

class let willBecomeActiveNotification: NSNotification.Name

Posted immediately before the app becomes active.

class let willResignActiveNotification: NSNotification.Name

Posted immediately before the app gives up its active status to another app.

class let willTerminateNotification: NSNotification.Name

Sends a notification to termintate the app.

class let columnConfigurationDidChangeNotification: NSNotification.Name

Notifies the delegate when the width of a browser column has changed.

static let NSClassDescriptionNeededForClass: NSNotification.Name

Posted by init(for:) when a class description cannot be found for a class.

static let NSApplicationProtectedDataDidBecomeAvailable: NSNotification.Name

static let NSApplicationProtectedDataWillBecomeUnavailable: NSNotification.Name

static let announcementRequested: NSAccessibility.Notification

This notification is posted whenever an accessibility element needs to make an announcement to the user. This notification requires a \`userInfo\` dictionary with the key and a localized string containing the announcement. To help an assistive app determine the importance of the announcement, add the appropriate to the \`userInfo\` dictionary.

static let applicationActivated: NSAccessibility.Notification

This notification is posted after the app has been activated. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let applicationDeactivated: NSAccessibility.Notification

This notification is posted after the app has been deactivated. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let applicationHidden: NSAccessibility.Notification

This notification is posted after the app is hidden. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let applicationShown: NSAccessibility.Notification

This notification is posted after the app is shown. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let created: NSAccessibility.Notification

This notification is posted after an accessibility element is created. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let drawerCreated: NSAccessibility.Notification

This notification is posted after a drawer appears. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let focusedUIElementChanged: NSAccessibility.Notification

This notification is posted after an accessibility element gains focus. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let focusedWindowChanged: NSAccessibility.Notification

This notification is posted after the key window changes. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let helpTagCreated: NSAccessibility.Notification

This notification is posted after a help tag appears. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let layoutChanged: NSAccessibility.Notification

This notification is posted after the UI changes in a way that requires the attention of an accessibility client. This notification should be accompanied by a \`userInfo\` dictionary with the key and an array containing the UI elements that have been added or changed. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let mainWindowChanged: NSAccessibility.Notification

This notification is posted after the main window changes. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let moved: NSAccessibility.Notification

This notification is posted after an accessibility element moves. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let resized: NSAccessibility.Notification

This notification is posted after an accessibility element’s size changes. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let rowCollapsed: NSAccessibility.Notification

This notification is posted after a row collapses. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let rowCountChanged: NSAccessibility.Notification

This notification is posted after a row is added or deleted. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let rowExpanded: NSAccessibility.Notification

This notification is posted after a row expands. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let selectedCellsChanged: NSAccessibility.Notification

This notification is posted after one or more cells in a cell-based table are selected or deselected. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let selectedChildrenChanged: NSAccessibility.Notification

This notification is posted after one or more child elements are selected or deselected. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let selectedChildrenMoved: NSAccessibility.Notification

This notification is posted after the selected items in a layout area move. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let selectedColumnsChanged: NSAccessibility.Notification

This notification is posted after one or more columns are selected or deselected. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let selectedRowsChanged: NSAccessibility.Notification

This notification is posted after one or more rows are selected or deselected. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let selectedTextChanged: NSAccessibility.Notification

This notification is posted after text is selected or deselected. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let sheetCreated: NSAccessibility.Notification

This notification is posted after a sheet appears. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let titleChanged: NSAccessibility.Notification

This notification is posted after an accessibility element’s title changes. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let uiElementDestroyed: NSAccessibility.Notification

This notification is posted after an accessibility element is destroyed. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let unitsChanged: NSAccessibility.Notification

This notification is posted after the units in a layout area change. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let valueChanged: NSAccessibility.Notification

This notification is posted after an accessibility element’s value changes. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let windowCreated: NSAccessibility.Notification

This notification is posted after a new window appears. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let windowDeminiaturized: NSAccessibility.Notification

This notification is posted after a window is restored to full size from the Dock. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let windowMiniaturized: NSAccessibility.Notification

This notification is posted after a window is put in the Dock. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let windowMoved: NSAccessibility.Notification

This notification is posted after a window moves. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

static let windowResized: NSAccessibility.Notification

This notification is posted after a window’s size changes. Post this notification using the function instead of an \`NSNotificationCenter\` instance.

class let progressMarkNotification: NSNotification.Name

Posted when the current progress of a running animation reaches one of its progress marks.

class let antialiasThresholdChangedNotification: NSNotification.Name

Posted after the threshold for antialiasing changes.

class let globalFrameDidChangeNotification: NSNotification.Name

Posted whenever an \`NSView\` object that has attached surfaces (that is, \`NSOpenGLContext\` objects) moves to a different screen, or other cases where the \`NSOpenGLContext\` object needs to be updated.

Deprecated

### AVFAudio

static let AVAudioEngineConfigurationChange: NSNotification.Name

A notification the framework posts when the audio engine configuration changes.

static let AVAudioUnitComponentTagsDidChange: NSNotification.Name

A notification that indicates when component tags change.

class let interruptionNotification: NSNotification.Name

A notification the system posts when an audio interruption occurs.

class let mediaServicesWereLostNotification: NSNotification.Name

A notification the system posts when it terminates the media server.

class let mediaServicesWereResetNotification: NSNotification.Name

A notification the system posts when the media server restarts.

class let routeChangeNotification: NSNotification.Name

A notification the system posts when its audio route changes.

class let silenceSecondaryAudioHintNotification: NSNotification.Name

A notification the system posts when the primary audio from other apps starts and stops.

### AVFoundation

static let AVAssetChapterMetadataGroupsDidChange: NSNotification.Name

A notification the system posts when an asset’s chapter metadata groups change.

static let AVAssetContainsFragmentsDidChange: NSNotification.Name

A notification the system posts when an asset’s fragments change.

static let AVAssetDurationDidChange: NSNotification.Name

A notification the system posts when a fragmented asset minder observes a change to a fragmented asset’s duration.

static let AVAssetMediaSelectionGroupsDidChange: NSNotification.Name

A notification the system posts when an asset’s media selection groups change.

static let AVAssetTrackSegmentsDidChange: NSNotification.Name

A notification the system posts when a fragmented asset minder observes a change to a fragmented asset track’s segments.

static let AVAssetTrackTimeRangeDidChange: NSNotification.Name

A notification the system posts when a fragmented asset minder observes a change to a fragmented asset track’s time range.

static let AVAssetTrackTrackAssociationsDidChange: NSNotification.Name

A notification the system posts when the track associations for an asset track change.

static let AVAssetWasDefragmented: NSNotification.Name

A notification the system posts when a fragmented asset minder observes that the system defragments the asset on disk.

class let subjectAreaDidChangeNotification: NSNotification.Name

A notification the system posts when a capture device detects a substantial change to the video subject area.

class let wasConnectedNotification: NSNotification.Name

A notification the system posts when a new capture device becomes available.

class let wasDisconnectedNotification: NSNotification.Name

A notification the system posts when an existing device becomes unavailable.

class let formatDescriptionDidChangeNotification: NSNotification.Name

A notification the system posts when the capture input port’s format description changes.

class let didStartRunningNotification: NSNotification.Name

A notification the system posts when a capture session starts.

class let didStopRunningNotification: NSNotification.Name

A notification the system posts when a capture session stops.

class let interruptionEndedNotification: NSNotification.Name

A notification the system posts when an interruption to a capture session finishes.

class let runtimeErrorNotification: NSNotification.Name

A notification the system posts when an error occurs during a capture session.

class let wasInterruptedNotification: NSNotification.Name

A notification the system posts when it interrupts a capture session.

static let AVFragmentedMovieContainsMovieFragmentsDidChange: NSNotification.Name

A notification the system posts when a fragmented movie minder observes a change to a movie’s fragments.

static let AVFragmentedMovieDurationDidChange: NSNotification.Name

A notification the system posts when a fragmented movie minder observes a change to a movie’s duration.

static let AVFragmentedMovieTrackSegmentsDidChange: NSNotification.Name

A notification the system posts when a fragmented movie minder observes a change to a fragmented movie track’s segments.

static let AVFragmentedMovieTrackTimeRangeDidChange: NSNotification.Name

A notification the system posts when a fragmented movie minder observes a change to a movie track’s time range.

static let AVFragmentedMovieWasDefragmented: NSNotification.Name

A notification the system posts when a fragmented movie minder observes that the system defragments the asset on disk.

static let AVPlayerAvailableHDRModesDidChange: NSNotification.Name

A notification the system posts when a player’s available HDR modes change.

Deprecated

class let assetListResponseStatusDidChangeNotification: NSNotification.Name

A notification the system posts when the status of an interstitial event’s asset list response changes.

class let didPlayToEndTimeNotification: NSNotification.Name

A notification the system posts when a player item plays to its end time.

class let failedToPlayToEndTimeNotification: NSNotification.Name

A notification that the system posts when a player item fails to play to its end time.

class let newAccessLogEntryNotification: NSNotification.Name

A notification the system posts when a player item adds a new entry to its access log.

class let newErrorLogEntryNotification: NSNotification.Name

A notification the system posts when a player item adds a new entry to its error log.

class let playbackStalledNotification: NSNotification.Name

A notification the system posts when a player item media doesn’t arrive in time to continue playback.

static let AVRouteDetectorMultipleRoutesDetectedDidChange: NSNotification.Name

A notification the system posts when changes occur to its detected routes.

static let AVSampleBufferAudioRendererOutputConfigurationDidChange: NSNotification.Name

A notification the system posts to indicate that the hardware configuration doesn’t match the enqueued data format.

static let AVSampleBufferAudioRendererWasFlushedAutomatically: NSNotification.Name

A notification the system posts when a renderer flushes its enqueued media data without an explicit request to do so.

static let AVSampleBufferDisplayLayerFailedToDecode: NSNotification.Name

A notification the system posts when a sample buffer display layer fails to decode.

static let AVSampleBufferDisplayLayerOutputObscuredDueToInsufficientExternalProtectionDidChange: NSNotification.Name

A notification the system posts when the current device configuration doesn’t support the external content protection mechanism.

static let AVSampleBufferDisplayLayerRequiresFlushToResumeDecodingDidChange: NSNotification.Name

A notification the system posts when a sample buffer display layer changes its decoding requirements.

class let timeJumpedNotification: NSNotification.Name

A notification the system posts when a player item’s time changes discontinuously.

static let AVFragmentedMovieTrackTotalSampleDataLengthDidChange: NSNotification.Name

A notification the system posts when the sample data length of a fragmented movie track changes.

Deprecated

static var AVPlayerItemTimeJumped: NSNotification.Name

A notification the system posts to indicate a jump in a player item’s current time.

Deprecated

class let timeJumpedNotification: NSNotification.Name

A notification the system posts when a player item’s time changes discontinuously.

### AVKit

static let AVDisplayManagerModeSwitchSettingsChanged: NSNotification.Name

A notification the display manager posts when a user changes their Match Content settings in the tvOS Settings app.

static let AVDisplayManagerModeSwitchStart: NSNotification.Name

A notification the display manager posts when a display begins a mode switch.

static let AVDisplayManagerModeSwitchEnd: NSNotification.Name

A notification the display manager posts when a display ends a mode switch.

### ClockKit

static let CLKComplicationServerActiveComplicationsDidChange: NSNotification.Name

Posted when the set of active complications changes.

Deprecated

### CloudKit

static let CKAccountChanged: NSNotification.Name

A notification that a container posts when the status of an iCloud account changes.

### Contacts

static let CNContactStoreDidChange: NSNotification.Name

Posted when changes occur to the contact store.

### Core Data

static let NSManagedObjectContextDidSave: NSNotification.Name

A notification that posts after a context finishes writing unsaved changes.

static let NSManagedObjectContextObjectsDidChange: NSNotification.Name

A notification that posts when there are changes to context’s registered managed objects.

static let NSManagedObjectContextWillSave: NSNotification.Name

A notification that posts before a context writes unsaved changes.

static let NSPersistentStoreCoordinatorStoresDidChange: NSNotification.Name

A notification that the coordinator posts after its registered stores change.

static let NSPersistentStoreCoordinatorStoresWillChange: NSNotification.Name

A notification that posts before a coordinator changes its registered stores.

static let NSPersistentStoreCoordinatorWillRemoveStore: NSNotification.Name

A notification that posts before a coordinator removes a store.

static let NSCoreDataCoreSpotlightDelegateIndexDidUpdate: NSNotification.Name

A notification that posts after Spotlight completes an index update.

static let NSManagedObjectContextDidMergeChangesObjectIDs: NSNotification.Name

A notification that posts after a context merges changes from a different notification.

static let NSManagedObjectContextDidSaveObjectIDs: NSNotification.Name

A notification that posts after a context finishes writing changes.

static let NSPersistentStoreRemoteChange: NSNotification.Name

A notification that posts after another process writes to a persistent store.

static let NSPersistentStoreDidImportUbiquitousContentChanges: NSNotification.Name

Posted after records are imported from the ubiquitous content store.

Deprecated

### Core Telephony

static let CTServiceRadioAccessTechnologyDidChange: NSNotification.Name

A notification that posts when radio access technology changes.

static let CTRadioAccessTechnologyDidChange: NSNotification.Name

The name of the notification indicating that the radio access technology changed for one of the services.

Deprecated

### Core WLAN

static let CWBSSIDDidChange: NSNotification.NameDeprecated

static let CWCountryCodeDidChange: NSNotification.NameDeprecated

static let CWLinkDidChange: NSNotification.NameDeprecated

static let CWLinkQualityDidChange: NSNotification.NameDeprecated

static let CWModeDidChange: NSNotification.NameDeprecated

static let CWPowerDidChange: NSNotification.NameDeprecated

static let CWSSIDDidChange: NSNotification.NameDeprecated

static let CWScanCacheDidUpdate: NSNotification.NameDeprecated

### EventKit

static let EKEventStoreChanged: NSNotification.Name

A notification posted when changes are made to the Calendar database.

### External Accessory

static let EAAccessoryDidConnect: NSNotification.Name

A notification that the system sends when an accessory becomes connected and available for your application to use.

static let EAAccessoryDidDisconnect: NSNotification.Name

A notification that is posted when an accessory is disconnected and no longer available for your application to use.

### File Provider

static let fileProviderDomainDidChange: NSNotification.Name

static let fileProviderMaterializedSetDidChange: NSNotification.Name

static let fileProviderPendingSetDidChange: NSNotification.Name

### Foundation

static let NSUbiquityIdentityDidChange: NSNotification.Name

Sent after the iCloud (“ubiquity”) identity has changed.

static let NSAppleEventManagerWillProcessFirstEvent: NSNotification.Name

Posted by `NSAppleEventManager` before it first dispatches an Apple event. Your application can use this notification to avoid registering any Apple event handlers until the first time at which they may be needed.

static let NSUndoManagerCheckpoint: NSNotification.Name

Posted whenever an undo manager opens or closes an undo group (except when it opens a top-level group) and when checking the redo stack.

static let NSUndoManagerDidCloseUndoGroup: NSNotification.Name

Posted after an undo manager closes an undo group.

static let NSUndoManagerDidOpenUndoGroup: NSNotification.Name

Posted whenever an undo manager opens an undo group.

static let NSUndoManagerDidRedoChange: NSNotification.Name

Posted just after an undo manager performs a redo operation.

static let NSUndoManagerDidUndoChange: NSNotification.Name

Posted just after an undo manager performs an undo operation.

static let NSUndoManagerWillCloseUndoGroup: NSNotification.Name

Posted before an undo manager closes an undo group.

static let NSUndoManagerWillRedoChange: NSNotification.Name

Posted just before an undo manager performs a redo operation.

static let NSUndoManagerWillUndoChange: NSNotification.Name

Posted just before an undo manager performs an undo operation.

static let NSWillBecomeMultiThreaded: NSNotification.Name

Posted when the first thread is detached from the current thread. The `NSThread` class posts this notification at most once—the first time a thread is detached using detachNewThreadSelector(_:toTarget:with:) or the start() method. Subsequent invocations of those methods do not post this notification. Observers of this notification have their notification method invoked in the main thread, not the new thread. The observer notification methods always execute before the new thread begins executing.

static let NSBundleResourceRequestLowDiskSpace: NSNotification.Name

Posted after the system detects that the amount of available disk space is getting low. The notification is posted to the default notification center.

static let NSCalendarDayChanged: NSNotification.Name

A notification that is posted whenever the calendar day of the system changes, as determined by the system calendar, locale, and time zone.

static let NSDidBecomeSingleThreaded: NSNotification.Name

Not implemented.

static let NSExtensionHostDidBecomeActive: NSNotification.Name

Posted when the extension’s host app moves from the inactive to the active state.

static let NSExtensionHostDidEnterBackground: NSNotification.Name

Posted when the extension’s host app begins running in the background.

static let NSExtensionHostWillEnterForeground: NSNotification.Name

Posted when the extension’s host app begins running in the foreground.

static let NSExtensionHostWillResignActive: NSNotification.Name

Posted when the extension’s host app moves from the active to the inactive state.

static let NSFileHandleConnectionAccepted: NSNotification.Name

Posted when a file handle object establishes a socket connection between two processes, creates a file handle object for one end of the connection, and makes this object available to observers.

static let NSFileHandleDataAvailable: NSNotification.Name

Posted when the file handle determines that data is currently available for reading in a file or at a communications channel.

static let NSFileHandleReadToEndOfFileCompletion: NSNotification.Name

Posted when the file handle reads all data in the file or, in a communications channel, until the other process signals the end of data.

static let NSHTTPCookieManagerAcceptPolicyChanged: NSNotification.Name

A notification posted when the acceptance policy of the cookie storage has changed.

static let NSHTTPCookieManagerCookiesChanged: NSNotification.Name

A notification posted when the cookies stored in the cookie storage have changed.

static let NSMetadataQueryDidFinishGathering: NSNotification.Name

Posted when the receiver has finished with the initial result-gathering phase of the query.

static let NSMetadataQueryDidStartGathering: NSNotification.Name

Posted when the receiver begins with the initial result-gathering phase of the query.

static let NSMetadataQueryDidUpdate: NSNotification.Name

Posted when the receiver’s results have changed during the live-update phase of the query.

static let NSMetadataQueryGatheringProgress: NSNotification.Name

Posted as the receiver is collecting results during the initial result-gathering phase of the query.

static let NSProcessInfoPowerStateDidChange: NSNotification.Name

Posts when the power state of a device changes.

static let NSSystemClockDidChange: NSNotification.Name

A notification posted whenever the system clock is changed.

static let NSSystemTimeZoneDidChange: NSNotification.Name

A notification posted when the time zone changes.

static let NSThreadWillExit: NSNotification.Name

An `NSThread` object posts this notification when it receives the exit() message, before the thread exits. Observer methods invoked to receive this notification execute in the exiting thread, before it exits.

static let NSURLCredentialStorageChanged: NSNotification.Name

A notification posted when the set of stored credentials changes.

### Game Controller

static let GCControllerDidConnect: NSNotification.Name

A notification that posts after a controller connects to the device.

static let GCControllerDidDisconnect: NSNotification.Name

A notification that posts after a controller disconnects from the device.

static let GCControllerDidBecomeCurrent: NSNotification.Name

A notification that posts when a controller becomes the current controller.

static let GCControllerDidStopBeingCurrent: NSNotification.Name

A notification that posts when a controller stops being the current controller.

static let GCControllerUserCustomizationsDidChange: NSNotification.Name

A notification that posts when the user customizes the button mappings or other settings of a controller.

static let GCKeyboardDidConnect: NSNotification.Name

A notification that posts after a keyboard connects to the device.

static let GCKeyboardDidDisconnect: NSNotification.Name

A notification that posts after a single keyboard, or the last of multiple keyboards, disconnects from the device.

static let GCMouseDidBecomeCurrent: NSNotification.Name

A notification that posts when a mouse becomes the most recent mouse that the user connects.

static let GCMouseDidConnect: NSNotification.Name

A notification that posts after a mouse connects to the device.

static let GCMouseDidDisconnect: NSNotification.Name

A notification that posts after a mouse disconnects from the device.

static let GCMouseDidStopBeingCurrent: NSNotification.Name

A notification that posts when a mouse stops being the most recent mouse that the user connects.

static let GCRacingWheelDidConnect: NSNotification.Name

A notification that posts after a racing wheel controller connects to the device.

static let GCRacingWheelDidDisconnect: NSNotification.Name

A notification that posts after a racing wheel controller disconnects from the device.

### GameKit

static let GKPlayerAuthenticationDidChangeNotificationName: NSNotification.Name

A notification that posts after GameKit authenticates the local player.

static let GKPlayerDidChangeNotificationName: NSNotification.Name

A notification that posts when a player object’s data changes.

### HealthKit

static let HKUserPreferencesDidChange: NSNotification.Name

Notifies observers whenever the user changes his or her preferred units.

### HomeKit

let HMCharacteristicPropertySupportsEventNotification: String

The characteristic supports event notifications.

### IOBluetooth

static let IOBluetoothHostControllerPoweredOff: NSNotification.Name

static let IOBluetoothHostControllerPoweredOn: NSNotification.Name

static let IOBluetoothL2CAPChannelPublished: NSNotification.Name

static let IOBluetoothL2CAPChannelTerminated: NSNotification.Name

### iTunes Library

static let ITLibraryDidChange: NSNotification.Name

A notification the system posts when a library change occurs.

### MapKit

static let MKAnnotationCalloutInfoDidChange: NSNotification.Name

A property to observe to determine when the title or subtitle information of an annotation object changes.

Deprecated

### MediaPlayer

static let MPMusicPlayerControllerQueueDidChange: NSNotification.Name

Indicates the music player’s queue changed.

static let MPMediaLibraryDidChange: NSNotification.Name

Indicates the media library has changed.

static let MPMediaPlaybackIsPreparedToPlayDidChange: NSNotification.Name

Indicates that the prepared to play status of the media player has changed.

Deprecated

static let MPMusicPlayerControllerNowPlayingItemDidChange: NSNotification.Name

Posted when the currently playing media item has changed.

static let MPMusicPlayerControllerPlaybackStateDidChange: NSNotification.Name

Posted when the playback state changes programmatically or by user action.

static let MPMusicPlayerControllerVolumeDidChange: NSNotification.Name

Posted when the audio playback volume for the music player has changed.

static let MPMovieDurationAvailable: NSNotification.Name

Posted when the duration of a movie has been determined. There is no `userInfo` dictionary.

Deprecated

static let MPMovieMediaTypesAvailable: NSNotification.Name

Posted when the available media types in a movie are determined. There is no `userInfo` dictionary.

Deprecated

static let MPMovieNaturalSizeAvailable: NSNotification.Name

Posted when the natural frame size of a movie is first determined or subsequently changes. There is no `userInfo` dictionary.

Deprecated

static let MPMoviePlayerDidEnterFullscreen: NSNotification.Name

Posted when a movie player has entered full-screen mode. There is no `userInfo` dictionary.

Deprecated

static let MPMoviePlayerDidExitFullscreen: NSNotification.Name

Posted when a movie player has exited full-screen mode. There is no `userInfo` dictionary.

Deprecated

static let MPMoviePlayerIsAirPlayVideoActiveDidChange: NSNotification.Name

Posted when a movie player has started or ended playing a movie via AirPlay. There is no `userInfo` dictionary.

Deprecated

static let MPMoviePlayerLoadStateDidChange: NSNotification.Name

Posted when a movie player’s network buffering state has changed. There is no `userInfo` dictionary.

Deprecated

static let MPMoviePlayerNowPlayingMovieDidChange: NSNotification.Name

Posted when the currently playing movie has changed. There is no `userInfo` dictionary.

Deprecated

static let MPMoviePlayerPlaybackDidFinish: NSNotification.Name

Posted when a movie has finished playing. The `userInfo` dictionary of this notification contains the MPMoviePlayerPlaybackDidFinishReasonUserInfoKey key, which indicates the reason that playback finished. This notification is also sent when playback fails because of an error.

Deprecated

static let MPMoviePlayerPlaybackStateDidChange: NSNotification.Name

Posted when a movie player’s playback state has changed. There is no `userInfo` dictionary.

Deprecated

static let MPMoviePlayerReadyForDisplayDidChange: NSNotification.Name

Posted when the ready for display state changes.

Deprecated

static let MPMoviePlayerScalingModeDidChange: NSNotification.Name

Posted when the scaling mode of a movie player has changed. There is no `userInfo` dictionary.

Deprecated

static let MPMoviePlayerThumbnailImageRequestDidFinish: NSNotification.Name

Posted when a request to capture a thumbnail from a movie has finished whether the request succeeded or failed. Upon successful capture of a thumbnail, the `userInfo` dictionary contains values for the following keys:

Deprecated

static let MPMoviePlayerTimedMetadataUpdated: NSNotification.Name

Posted when new timed metadata arrives.

Deprecated

static let MPMoviePlayerWillEnterFullscreen: NSNotification.Name

Posted when a movie player is about to enter full-screen mode. The `userInfo` dictionary contains keys whose values describe the transition animation used to enter full-screen mode. See Fullscreen notification keys.

Deprecated

static let MPMoviePlayerWillExitFullscreen: NSNotification.Name

Posted when a movie player is about to exit full-screen mode. The `userInfo` dictionary contains keys whose values describe the transition animation used to exit full-screen mode. See Fullscreen notification keys.

Deprecated

static let MPMovieSourceTypeAvailable: NSNotification.Name

Posted when the source type of a movie was previously unknown and is newly available. There is no `userInfo` dictionary.

Deprecated

static let MPVolumeViewWirelessRouteActiveDidChange: NSNotification.Name

Indicates the active wireless route changed.

Deprecated

static let MPVolumeViewWirelessRoutesAvailableDidChange: NSNotification.Name

Indicates the available wireless routes changed.

Deprecated

### MessageUI

static let MFMessageComposeViewControllerTextMessageAvailabilityDidChange: NSNotification.Name

Posted when the value returned by the canSendText() class method has changed.

MFMessageComposeViewControllerTextMessageAvailabilityDidChangeNotification

Posted when the value returned by the class method has changed.

### NetworkExtension

static let NEFilterConfigurationDidChange: NSNotification.Name

Posted after the filter configuration stored in the Network Extension preferences changes.

static let NEVPNConfigurationChange: NSNotification.Name

Posted after the VPN configuration stored in the Network Extension preferences changes.

static let NEVPNStatusDidChange: NSNotification.Name

Posted when the status of the VPN connection changes.

static let NEDNSProxyConfigurationDidChange: NSNotification.Name

A notification that is posted when the DNS proxy configuration changes.

static let NEDNSSettingsConfigurationDidChange: NSNotification.Name

### PassKit

static let PKPassLibraryDidChange: PKPassLibraryNotificationName

A notification that PassKit posts when the pass library changes.

static let PKPassLibraryRemotePaymentPassesDidChange: PKPassLibraryNotificationName

A notification that PassKit posts when it adds or removes a pass on a paired remote device.

### PDFKit

static let PDFDocumentDidBeginFind: NSNotification.Name

A notification that the beginFindString(_:withOptions:) or findString(_:withOptions:) method begins finding.

static let PDFDocumentDidBeginPageFind: NSNotification.Name

A notification that a find operation begins working on a new page of a document.

static let PDFDocumentDidBeginPageWrite: NSNotification.Name

A notification that a write operation begins working on a page in a document.

static let PDFDocumentDidBeginWrite: NSNotification.Name

A notification that a write operation begins working on a document.

static let PDFDocumentDidEndFind: NSNotification.Name

A notification that the beginFindString(_:withOptions:) or findString(_:withOptions:) method returns.

static let PDFDocumentDidEndPageFind: NSNotification.Name

A notification that a find operation finishes working on a page in a document.

static let PDFDocumentDidEndPageWrite: NSNotification.Name

A notification that a write operation finishes working on a page in a document.

static let PDFDocumentDidEndWrite: NSNotification.Name

A notification that a write operation finishes working on a document.

static let PDFDocumentDidFindMatch: NSNotification.Name

A notification that a string match is found in a document.

static let PDFDocumentDidUnlock: NSNotification.Name

A notification that a document unlocks after a unlock(withPassword:) message.

static let PDFThumbnailViewDocumentEdited: NSNotification.Name

static let PDFViewAnnotationHit: NSNotification.Name

A notification posted when the user clicks on an annotation.

static let PDFViewAnnotationWillHit: NSNotification.Name

A notification posted before the user clicks an annotation.

static let PDFViewChangedHistory: NSNotification.Name

A notification posted when the page history changes.

static let PDFViewCopyPermission: NSNotification.Name

A notification posted when the user attempts to copy to the pasteboard without the appropriate permissions.

static let PDFViewDisplayBoxChanged: NSNotification.Name

A notification posted when the display box has changed.

static let PDFViewDisplayModeChanged: NSNotification.Name

A notification posted when the display mode has changed.

static let PDFViewDocumentChanged: NSNotification.Name

A notification posted when a new document is associated with the view.

static let PDFViewPageChanged: NSNotification.Name

A notification posted when a new page becomes the current page.

static let PDFViewPrintPermission: NSNotification.Name

A notification posted when the user attempts to print without the appropriate permissions.

static let PDFViewScaleChanged: NSNotification.Name

A notification posted when the scale factor changes.

static let PDFViewSelectionChanged: NSNotification.Name

A notification posted when the current selection has changed.

static let PDFViewVisiblePagesChanged: NSNotification.Name

A notification posted when the visible pages have changed.

### PreferencePanes

static let NSPreferencePaneCancelUnselect: NSNotification.Name

Notifies observers that the preference pane should not be deselected.

static let NSPreferencePaneDoUnselect: NSNotification.Name

Notifies observers that the preference pane may be deselected.

static let NSPreferencePaneSwitchToPane: NSNotification.Name

Notifies observers that the user selected a new preference pane.

static let NSPreferencePaneUpdateHelpMenu: NSNotification.Name

Notifies observers that your help menu content changed.

static let NSPreferencePrefPaneIsAvailable: NSNotification.Name

Notifies observers that the system preferences app is available to display your preferences.

### Quartz

static let IKFilterBrowserFilterDoubleClick: NSNotification.Name

Posted when the user double-clicks a filter in the filter browser.

static let IKFilterBrowserFilterSelected: NSNotification.Name

Posted when the user clicks a filter name in the filter browser.

static let IKFilterBrowserWillPreviewFilter: NSNotification.Name

Posted before showing a filter preview, allowing an application to set the parameters of a filter.

static let quartzFilterManagerDidAddFilter: NSNotification.Name

static let quartzFilterManagerDidModifyFilter: NSNotification.Name

static let quartzFilterManagerDidRemoveFilter: NSNotification.Name

static let quartzFilterManagerDidSelectFilter: NSNotification.Name

static let QCCompositionPickerPanelDidSelectComposition: NSNotification.Name

Posted when the user chooses a composition.

Deprecated

static let QCCompositionPickerViewDidSelectComposition: NSNotification.Name

Posted when the user selects a composition in the picker view.

Deprecated

static let QCCompositionRepositoryDidUpdate: NSNotification.Name

Posted whenever the list of compositions in the composition repository is updated.

Deprecated

static let QCViewDidStartRendering: NSNotification.Name

Posted when the view starts rendering.

Deprecated

static let QCViewDidStopRendering: NSNotification.Name

Posted when the view stops rendering.

Deprecated

### StoreKit

static let SKCloudServiceCapabilitiesDidChange: NSNotification.Name

A notification name for indicating a change in the capabilities associated with the Music library on the device.

Deprecated

static let SKStorefrontIdentifierDidChange: NSNotification.Name

A notification name for indicating a change in the storefront identifier associated with the device.

Deprecated

static let SKStorefrontCountryCodeDidChange: NSNotification.Name

A notification name for indicating a change in the storefront country or region code associated with the device.

Deprecated

### TV Services

static let TVTopShelfItemsDidChange: NSNotification.Name

A notification to post when your app’s Top Shelf content has changed.

Deprecated

### UIKit

nonisolated static let announcementDidFinishNotification: NSNotification.Name

A notification that UIKit posts when the system finishes reading an announcement.

nonisolated static let elementFocusedNotification: NSNotification.Name

A notification that UIKit posts when an assistive app focuses on an accessibility element.

nonisolated static let assistiveTouchStatusDidChangeNotification: NSNotification.Name

A notification that indicates a change in the status of AssistiveTouch.

nonisolated static let boldTextStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Bold Text setting changes.

nonisolated static let closedCaptioningStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the setting for Closed Captions + SDH changes.

nonisolated static let darkerSystemColorsStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Increase Contrast setting changes.

nonisolated static let grayscaleStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Grayscale setting changes.

nonisolated static let guidedAccessStatusDidChangeNotification: NSNotification.Name

A notification that indicates when a Guided Access session starts or ends.

nonisolated static let hearingDevicePairedEarDidChangeNotification: NSNotification.Name

A notification that UIKit posts when there’s a change to the currently paired hearing devices.

nonisolated static let invertColorsStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the settings for inverted colors change.

nonisolated static let monoAudioStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when system audio changes from stereo to mono.

nonisolated static let reduceMotionStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Reduce Motion setting changes.

nonisolated static let reduceTransparencyStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Reduce Transparency setting changes.

nonisolated static let shakeToUndoDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Shake to Undo setting changes.

nonisolated static let speakScreenStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Speak Screen setting changes.

nonisolated static let speakSelectionStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Speak Selection setting changes.

nonisolated static let switchControlStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Switch Control setting changes.

nonisolated class let didBecomeActiveNotification: NSNotification.Name

A notification that posts when the app becomes active.

nonisolated class let didEnterBackgroundNotification: NSNotification.Name

A notification that posts when the app enters the background.

nonisolated class let didFinishLaunchingNotification: NSNotification.Name

A notification that posts immediately after the app finishes launching.

nonisolated class let didReceiveMemoryWarningNotification: NSNotification.Name

A notification that posts when the app receives a warning from the operating system about low memory availability.

nonisolated class let significantTimeChangeNotification: NSNotification.Name

A notification that posts when there’s a significant change in time.

nonisolated class let userDidTakeScreenshotNotification: NSNotification.Name

A notification that posts when a person takes a screenshot on the device.

nonisolated class let willEnterForegroundNotification: NSNotification.Name

A notification that posts shortly before an app leaves the background state on its way to becoming the active app.

nonisolated class let willResignActiveNotification: NSNotification.Name

A notification that posts when the app is no longer active and loses focus.

nonisolated class let willTerminateNotification: NSNotification.Name

A notification that posts when the app is about to terminate.

nonisolated static let didChangeNotification: NSNotification.Name

A notification that posts when the user changes the preferred content size setting.

nonisolated class let proximityStateDidChangeNotification: NSNotification.Name

A notification that posts when the state of the proximity sensor changes.

nonisolated class let brightnessDidChangeNotification: NSNotification.Name

A notification that posts when a screen’s brightness changes.

nonisolated class let didConnectNotification: NSNotification.Name

A notification the system posts when a new screen connects to the device.

Deprecated

nonisolated class let didDisconnectNotification: NSNotification.Name

A notification the system posts when a screen disconnects from the device.

Deprecated

nonisolated class let modeDidChangeNotification: NSNotification.Name

A notification that posts when a screen’s mode changes.

nonisolated class let selectionDidChangeNotification: NSNotification.Name

A notification that posts when the selected row in the posting table view changes.

nonisolated class let textDidBeginEditingNotification: NSNotification.Name

A notification that alerts observers when an editing session begins in a text field.

nonisolated class let textDidChangeNotification: NSNotification.Name

A notification that alerts observers when the text in a text field changes.

nonisolated class let textDidEndEditingNotification: NSNotification.Name

A notification that alerts observers when the editing session ends for a text field.

nonisolated class let currentInputModeDidChangeNotification: NSNotification.Name

A notification that posts when the current input mode changes.

nonisolated class let textDidBeginEditingNotification: NSNotification.Name

A notification that alerts observers when an editing session begins in a text view.

nonisolated class let textDidChangeNotification: NSNotification.Name

A notification that alerts observers when the text in a text view changes.

nonisolated class let textDidEndEditingNotification: NSNotification.Name

A notification that alerts observers when the editing session ends for a text view.

nonisolated class let showDetailTargetDidChangeNotification: NSNotification.Name

Posted when a split view controller is expanded or collapsed.

nonisolated class let didBecomeHiddenNotification: NSNotification.Name

A notification that posts when a window becomes hidden.

nonisolated class let didBecomeKeyNotification: NSNotification.Name

A notification that posts whenever a window becomes the key window.

nonisolated class let didBecomeVisibleNotification: NSNotification.Name

A notification that posts when a window becomes visible.

nonisolated class let didResignKeyNotification: NSNotification.Name

A notification that posts whenever a window resigns its status as main window.

nonisolated class let backgroundRefreshStatusDidChangeNotification: NSNotification.Name

A notification that posts when the app’s status for downloading content in the background changes.

nonisolated class let didChangeStatusBarFrameNotification: NSNotification.Name

Posted when the frame of the status bar changes.

Deprecated

nonisolated class let didChangeStatusBarOrientationNotification: NSNotification.Name

Posted when the orientation of the app’s user interface changes.

Deprecated

nonisolated class let willChangeStatusBarFrameNotification: NSNotification.Name

Posted when the app is about to change the frame of the status bar.

Deprecated

nonisolated class let willChangeStatusBarOrientationNotification: NSNotification.Name

Posted when the app is about to change the orientation of its interface.

Deprecated

nonisolated class let batteryLevelDidChangeNotification: NSNotification.Name

A notification that posts when the battery level changes.

nonisolated class let batteryStateDidChangeNotification: NSNotification.Name

A notification that posts when battery state changes.

nonisolated class let orientationDidChangeNotification: NSNotification.Name

A notification that posts when the orientation of the device changes.

nonisolated class let stateChangedNotification: NSNotification.Name

A notification the document object posts when there’s a change in the state of the document.

nonisolated class let keyboardDidChangeFrameNotification: NSNotification.Name

A notification that posts immediately after a change in the keyboard’s frame.

nonisolated class let keyboardDidHideNotification: NSNotification.Name

A notification that posts immediately after dismissing the keyboard.

nonisolated class let keyboardDidShowNotification: NSNotification.Name

A notification that posts immediately after displaying the keyboard.

nonisolated class let keyboardWillChangeFrameNotification: NSNotification.Name

A notification that posts immediately prior to a change in the keyboard’s frame.

nonisolated class let keyboardWillHideNotification: NSNotification.Name

A notification that posts immediately prior to dismissing the keyboard.

nonisolated class let keyboardWillShowNotification: NSNotification.Name

A notification that posts immediately prior to displaying the keyboard.

nonisolated class let didHideMenuNotification: NSNotification.Name

Posted by the menu controller just after it hides the menu.

Deprecated

nonisolated class let didShowMenuNotification: NSNotification.Name

Posted by the menu controller just after it shows the menu.

Deprecated

nonisolated class let menuFrameDidChangeNotification: NSNotification.Name

Posted when the frame of a visible menu changes.

Deprecated

nonisolated class let willHideMenuNotification: NSNotification.Name

Posted by the menu controller just before it hides the menu.

Deprecated

nonisolated class let willShowMenuNotification: NSNotification.Name

Posted by the menu controller just before it shows the menu.

Deprecated

nonisolated class let changedNotification: NSNotification.Name

A notification that a pasteboard object posts when its contents change.

nonisolated class let removedNotification: NSNotification.Name

A notification that a pasteboard object posts just before an app removes it.

nonisolated class let protectedDataDidBecomeAvailableNotification: NSNotification.Name

A notification that posts when the protected files become available for your code to access.

nonisolated class let protectedDataWillBecomeUnavailableNotification: NSNotification.Name

A notification that posts shortly before protected files are locked down and become inaccessible.

### WatchKit

static let WKAccessibilityReduceMotionStatusDidChange: NSNotification.Name

Tells the interface controller that the reduce motion status has changed.

static let WKAudioFilePlayerItemDidPlayToEndTime: NSNotification.Name

A notification that the item has played successfully to its end.

Deprecated

static let WKAudioFilePlayerItemFailedToPlayToEndTime: NSNotification.Name

A notification that the item failed to play to its end.

Deprecated

static let WKAudioFilePlayerItemTimeJumped: NSNotification.Name

A notification that the item’s current time has changed discontinuously.

Deprecated

### WebKit

static let WebHistoryAllItemsRemoved: NSNotification.Name

Posted when all history items have been removed from the web history.

Deprecated

static let WebHistoryItemChanged: NSNotification.Name

Posted by a WebHistoryItem object when the value of the history item’s title, alternate title, URL strings, or last visited interval changes.

Deprecated

static let WebHistoryItemsAdded: NSNotification.Name

Posted when history items have been added to a web history.

Deprecated

static let WebHistoryItemsRemoved: NSNotification.Name

Posted when items have been removed from the web history.

Deprecated

static let WebHistoryLoaded: NSNotification.Name

Posted when web history items have been loaded from a URL.

Deprecated

static let WebHistorySaved: NSNotification.Name

Posted when web history items have been saved to a URL.

Deprecated

static let WebPreferencesChanged: NSNotification.Name

Posted when the web preference settings are changed.

Deprecated

static let WebViewDidBeginEditing: NSNotification.Name

Posted when a web view begins any operation that changes its contents in response to user editing.

Deprecated

static let WebViewDidChange: NSNotification.Name

Posted when a web view performs any operation that changes its contents in response to user editing.

Deprecated

static let WebViewDidChangeSelection: NSNotification.Name

Posted when a web view changes its typing selection.

Deprecated

static let WebViewDidChangeTypingStyle: NSNotification.Name

Posted when a web view changes its typing style.

Deprecated

static let WebViewDidEndEditing: NSNotification.Name

Posted when a web view ends any operation that changes its contents in response to user editing.

Deprecated

static let WebViewProgressEstimateChanged: NSNotification.Name

Posted by a WebView object when the estimated progress value of a load changes.

Deprecated

static let WebViewProgressFinished: NSNotification.Name

Posted by a WebView object when the load has finished.

Deprecated

static let WebViewProgressStarted: NSNotification.Name

Posted by a WebView object when a load begins, including a load that is initiated in a subframe.

Deprecated

### Accounts

static let ACAccountStoreDidChange: NSNotification.Name

Posted when the accounts managed by this account store changed in the database.

Deprecated

### AssetsLibrary

static let ALAssetsLibraryChanged: NSNotification.Name

Sent when the contents of the assets library have changed from under the app that is using the data.

Deprecated

### Initializers

init(String)

init(rawValue: String)

### Type Properties

static var AVCaptureDeviceSubjectAreaDidChange: NSNotification.NameDeprecated

static var AVCaptureDeviceWasConnected: NSNotification.NameDeprecated

static var AVCaptureDeviceWasDisconnected: NSNotification.NameDeprecated

static var AVCaptureInputPortFormatDescriptionDidChange: NSNotification.NameDeprecated

static var AVCaptureSessionDidStartRunning: NSNotification.NameDeprecated

static var AVCaptureSessionDidStopRunning: NSNotification.NameDeprecated

static var AVCaptureSessionInterruptionEnded: NSNotification.NameDeprecated

static var AVCaptureSessionRuntimeError: NSNotification.NameDeprecated

static var AVCaptureSessionWasInterrupted: NSNotification.NameDeprecated

static var AVPlayerInterstitialEventMonitorAssetListResponseStatusDidChange: NSNotification.NameDeprecated

static var AVPlayerItemDidPlayToEndTime: NSNotification.NameDeprecated

static var AVPlayerItemFailedToPlayToEndTime: NSNotification.NameDeprecated

static var AVPlayerItemNewAccessLogEntry: NSNotification.NameDeprecated

static var AVPlayerItemNewErrorLogEntry: NSNotification.NameDeprecated

static var AVPlayerItemPlaybackStalled: NSNotification.NameDeprecated

static let AVSampleBufferDisplayLayerReadyForDisplayDidChange: NSNotification.Name

static let AXAnimatedImagesEnabledDidChange: Notification.Name

static let AXPrefersHeadAnchorAlternativeDidChange: Notification.NameDeprecated

static let AXPrefersHorizontalTextLayoutDidChange: Notification.Name

static let DRBurnProgressPanelDidFinish: NSNotification.Name

static let DRBurnProgressPanelWillBegin: NSNotification.Name

static let DRBurnStatusChanged: NSNotification.Name

static let DRDeviceAppeared: NSNotification.Name

static let DRDeviceDisappeared: NSNotification.Name

static let DRDeviceStatusChanged: NSNotification.Name

static let DREraseProgressPanelDidFinish: NSNotification.Name

static let DREraseProgressPanelWillBegin: NSNotification.Name

static let DREraseStatusChanged: NSNotification.Name

static let DRSetupPanelDeviceSelectionChanged: NSNotification.Name

static let HMCharacteristicPropertySupportsEvent: NSNotification.Name

static let JRSMenuDidReuseItem: NSNotification.NameDeprecated

static let MEVideoDecoderReadyForMoreMediaDataDidChange: NSNotification.Name

static let NERelayConfigurationDidChange: NSNotification.Name

static let NSProcessInfoPerformanceProfileDidChange: NSNotification.Name

static let NSSpellCheckerDidChangeAutomaticInlinePrediction: NSNotification.Name

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating Notifications

init?(coder: NSCoder)

Initializes a notification with the data from an unarchiver.

convenience init(name: NSNotification.Name, object: Any?)

Returns a new notification object with a specified name and object.

init(name: NSNotification.Name, object: Any?, userInfo: [AnyHashable : Any]?)

Initializes a notification with a specified name, object, and user information.

