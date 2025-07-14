

- AppKit
- NSImage
-  NSImage.Name 

Type Alias

# NSImage.Name

Named images, defined by the system or you, for use in your app.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
typealias Name = String
```

## Discussion

The appearance of system-supplied images can change between releases. If you use an image for its intended purpose (and not because of how it looks), your code should look correct from release to release.

The size and aspect ratio of system images can also change between releases. In some situations, you should explicitly resize images as appropriate for your use. If you use these images in conjunction with an NSButtonCell object, however, you can use the imageScaling property of the cell to control scaling instead. Similarly, for an NSSegmentedCell object, you can use the setImageScaling(_:forSegment:): method to control scaling.

Constants that end in the word “Template” represent template images. These images can be processed into variants appropriate for different situations. For example, these images can invert in a selected table view row. See isTemplate for more information.

Some images also contain the word “FreestandingTemplate”. These images are template images that are appropriate for use as a borderless button—that is, it doesn’t need any extra bezel artwork behind it.

## Topics

### System Images

class let actionTemplateName: String

An action menu template image.

class let addTemplateName: String

An add item template image.

class let advancedName: String

Advanced preferences toolbar icon for the preferences window.

class let applicationIconName: String

The app’s icon.

class let bluetoothTemplateName: String

A Bluetooth template image.

class let bonjourName: String

A Bonjour icon.

class let bookmarksTemplateName: String

Bookmarks image suitable for a template.

class let cautionName: String

A caution image.

class let colorPanelName: String

A color panel toolbar icon.

class let columnViewTemplateName: String

A column view mode template image.

class let computerName: String

A computer icon.

class let enterFullScreenTemplateName: String

An enter full-screen mode template image.

class let everyoneName: String

Permissions for all users.

class let exitFullScreenTemplateName: String

An exit full-screen mode template image.

class let flowViewTemplateName: String

A cover flow view mode template image.

class let folderName: String

A folder image.

class let folderBurnableName: String

A burnable folder icon.

class let folderSmartName: String

A smart folder icon.

class let followLinkFreestandingTemplateName: String

A link template image.

class let fontPanelName: String

A font panel toolbar icon.

class let goBackTemplateName: String

A “go back” template image.

class let goForwardTemplateName: String

A “go forward” template image.

class let goLeftTemplateName: String

A “go back” template image.

class let goRightTemplateName: String

A “go forward” template image.

class let homeTemplateName: String

Home image suitable for a template.

class let iChatTheaterTemplateName: String

An iChat Theater template image.

class let iconViewTemplateName: String

An icon view mode template image.

class let infoName: String

An information toolbar icon.

class let invalidDataFreestandingTemplateName: String

A template image used to denote invalid data.

class let leftFacingTriangleTemplateName: String

A generic left-facing triangle template image.

class let listViewTemplateName: String

A list view mode template image.

class let lockLockedTemplateName: String

A locked padlock template image.

class let lockUnlockedTemplateName: String

An unlocked padlock template image.

class let menuMixedStateTemplateName: String

A horizontal dash, for use in menus.

class let menuOnStateTemplateName: String

A check mark template image, for use in menus.

class let mobileMeName: String

A MobileMe icon.

class let multipleDocumentsName: String

A drag image for multiple items.

class let networkName: String

A network icon.

class let pathTemplateName: String

A path button template image.

class let preferencesGeneralName: String

General preferences toolbar icon for the preferences window.

class let quickLookTemplateName: String

A Quick Look template image.

class let refreshFreestandingTemplateName: String

A refresh template image.

class let refreshTemplateName: String

A refresh template image.

class let removeTemplateName: String

A remove item template image.

class let revealFreestandingTemplateName: String

A reveal contents template image.

class let rightFacingTriangleTemplateName: String

A generic right-facing triangle template image.

class let shareTemplateName: String

A share view template image.

class let slideshowTemplateName: String

A slideshow template image.

class let smartBadgeTemplateName: String

A badge for a “smart” item.

class let statusAvailableName: String

Small green indicator, similar to iChat’s available image.

class let statusNoneName: String

Small clear indicator.

class let statusPartiallyAvailableName: String

Small yellow indicator, similar to iChat’s idle image.

class let statusUnavailableName: String

Small red indicator, similar to iChat’s unavailable image.

class let stopProgressFreestandingTemplateName: String

A stop progress template image.

class let stopProgressTemplateName: String

A stop progress button template image.

class let touchBarAddDetailTemplateName: String

A template image for showing additional detail for an item.

class let touchBarAddTemplateName: String

A template image for creating a new item.

class let touchBarAlarmTemplateName: String

A template image for setting or showing an alarm.

class let touchBarAudioInputMuteTemplateName: String

A template image for muting audio input or denoting that audio input is muted.

class let touchBarAudioInputTemplateName: String

A template image for denoting audio input.

class let touchBarAudioOutputMuteTemplateName: String

A template image for muting audio output or for denoting that audio output is muted.

class let touchBarAudioOutputVolumeHighTemplateName: String

A template image for setting the audio output volume to a high level, or for denoting that the audio is at the peak volume.

class let touchBarAudioOutputVolumeLowTemplateName: String

A template image for setting the audio output volume to a low level, or for denoting that it is set to a low level.

class let touchBarAudioOutputVolumeMediumTemplateName: String

A template image for setting the audio output volume to a medium level, or for denoting that it is set to a medium level.

class let touchBarAudioOutputVolumeOffTemplateName: String

A template image for setting the audio output volume to silent, or for denoting that it is set to silent.

class let touchBarBookmarksTemplateName: String

A template image for showing app-specific bookmarks.

class let touchBarColorPickerFillName: String

A template image for showing a color picker so the user can select a fill color.

class let touchBarColorPickerFontName: String

A template image for showing a color picker so the user can select a text color.

class let touchBarColorPickerStrokeName: String

A template image for showing a color picker so the user can select a stroke color.

class let touchBarCommunicationAudioTemplateName: String

A template image for initiating or denoting audio communication.

class let touchBarCommunicationVideoTemplateName: String

A template image for initiating or denoting video communication.

class let touchBarComposeTemplateName: String

A template image for opening a new document or view in edit mode.

class let touchBarDeleteTemplateName: String

A template image for deleting the current or selected item.

class let touchBarDownloadTemplateName: String

A template image for downloading an item.

class let touchBarEnterFullScreenTemplateName: String

A template image for entering full screen mode.

class let touchBarExitFullScreenTemplateName: String

A template image for exiting full screen mode.

class let touchBarFastForwardTemplateName: String

A template image for moving forward through media playback or slides.

class let touchBarFolderCopyToTemplateName: String

A template image for copying an item to a destination.

class let touchBarFolderMoveToTemplateName: String

A template image for moving an item to a destination.

class let touchBarFolderTemplateName: String

A template image for opening or representing a folder.

class let touchBarGetInfoTemplateName: String

A template image for showing information about an item.

class let touchBarGoBackTemplateName: String

A template image for returning to the previous screen or location.

class let touchBarGoDownTemplateName: String

A template image for moving to the next item in a list.

class let touchBarGoForwardTemplateName: String

A template image for moving to the next screen or location.

class let touchBarGoUpTemplateName: String

A template image for moving to the previous item in a list.

class let touchBarHistoryTemplateName: String

A template image for showing history information, such as recent downloads.

class let touchBarIconViewTemplateName: String

A template image for showing items in an icon view.

class let touchBarListViewTemplateName: String

A template image for showing items in a list view.

class let touchBarMailTemplateName: String

A template image for creating an email message.

class let touchBarNewFolderTemplateName: String

A template image for creating a new folder.

class let touchBarNewMessageTemplateName: String

A template image for creating a new message, or for denoting the use of messaging.

class let touchBarOpenInBrowserTemplateName: String

A template image for opening an item in the user’s browser.

class let touchBarPauseTemplateName: String

A template image for pausing media playback or slides.

class let touchBarPlayPauseTemplateName: String

A template image for toggling between playing and pausing media or slides.

class let touchBarPlayTemplateName: String

A template image for starting or resuming playback of media or slides.

class let touchBarPlayheadTemplateName: String

A template image for denoting the current playback position within a timeline track.

class let touchBarQuickLookTemplateName: String

A template image for opening an item in Quick Look.

class let touchBarRecordStartTemplateName: String

A template image for starting recording.

class let touchBarRecordStopTemplateName: String

A template image for stopping recording or stopping playback of media or slides.

class let touchBarRefreshTemplateName: String

A template image for refreshing displayed data.

class let touchBarRemoveTemplateName: String

A template image for removing an item.

class let touchBarRewindTemplateName: String

A template image for moving backwards through media or slides.

class let touchBarRotateLeftTemplateName: String

A template image for rotating an item counterclockwise.

class let touchBarRotateRightTemplateName: String

A template image for rotating an item clockwise.

class let touchBarSearchTemplateName: String

A template image for showing a search field or for initiating a search.

class let touchBarShareTemplateName: String

A template image for sharing content with others directly or via social media.

class let touchBarSidebarTemplateName: String

A template image for showing a sidebar in the current view.

class let touchBarSkipAhead15SecondsTemplateName: String

A template image for skipping ahead 15 seconds during media playback.

class let touchBarSkipAhead30SecondsTemplateName: String

A template image for skipping ahead 30 seconds during media playback.

class let touchBarSkipAheadTemplateName: String

A template image for skipping to the next chapter or location during media playback.

class let touchBarSkipBack15SecondsTemplateName: String

A template image for skipping back 15 seconds during media playback.

class let touchBarSkipBack30SecondsTemplateName: String

A template image for skipping back 30 seconds during media playback.

class let touchBarSkipBackTemplateName: String

A template image for skipping to the previous chapter or location during media playback.

class let touchBarSkipToEndTemplateName: String

A template image for skipping to the end of media playback.

class let touchBarSkipToStartTemplateName: String

A template image for skipping to the start of media playback.

class let touchBarSlideshowTemplateName: String

A template image for starting a slideshow.

class let touchBarTagIconTemplateName: String

A template image for applying a tag to an item.

class let touchBarTextBoldTemplateName: String

A template image for making selected text bold.

class let touchBarTextBoxTemplateName: String

A template image for inserting a text box.

class let touchBarTextCenterAlignTemplateName: String

A template image for centering text.

class let touchBarTextItalicTemplateName: String

A template image for italicizing the selected text.

class let touchBarTextJustifiedAlignTemplateName: String

A template image for fully justifying text.

class let touchBarTextLeftAlignTemplateName: String

A template image for aligning text to the left.

class let touchBarTextListTemplateName: String

A template image for inserting a list or converting text to list form.

class let touchBarTextRightAlignTemplateName: String

A template image for aligning text to the right.

class let touchBarTextStrikethroughTemplateName: String

A template image for striking through text.

class let touchBarTextUnderlineTemplateName: String

A template image for underlining text.

class let touchBarUserAddTemplateName: String

A template image for creating a new user account.

class let touchBarUserGroupTemplateName: String

A template image for showing or representing a group of users.

class let touchBarUserTemplateName: String

A template image for showing or representing user information.

class let touchBarVolumeDownTemplateName: String

A template image for reducing the audio output volume.

class let touchBarVolumeUpTemplateName: String

A template image for increasing the audio output volume.

class let trashEmptyName: String

An image of the empty trash can.

class let trashFullName: String

An image of the full trash can.

class let userName: String

Permissions for a single user.

class let userAccountsName: String

User account toolbar icon for the preferences window.

class let userGroupName: String

Permissions for a group of users.

class let userGuestName: String

Permissions for guests.

## See Also

### Creating Images by Name

Configuring and displaying symbol images in your UI

Create scalable images that integrate with your app’s text, and adjust the appearance of those images dynamically.

init?(named: NSImage.Name)

Returns the image object associated with the specified name.

convenience init?(systemSymbolName: String, accessibilityDescription: String?)

Creates a symbol image with the system symbol name and accessibility description you specify.

convenience init?(systemSymbolName: String, variableValue: Double, accessibilityDescription: String?)

Creates a symbol image with the system symbol name and variable value you specify.

convenience init?(symbolName: String, variableValue: Double)

Creates a symbol image with the symbol name and variable value you specify.

convenience init?(symbolName: String, bundle: Bundle?, variableValue: Double)

convenience init(resource: ImageResource)

func setName(NSImage.Name?) -> Bool

Registers the image object under the specified name.

func name() -> NSImage.Name?

Returns the name associated with the image, if any.

convenience init(imageLiteralResourceName: String)

Creates an image initialized with the specified resource name.

