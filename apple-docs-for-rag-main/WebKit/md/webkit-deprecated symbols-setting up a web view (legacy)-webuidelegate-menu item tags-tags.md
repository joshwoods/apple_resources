

- WebKit
- Deprecated Symbols
- Setting Up a Web View (Legacy)
- WebUIDelegate
-  Menu Item Tags 

API Collection

# Menu Item Tags

Tags that define the types of default menu items passed to the webView(_:contextMenuItemsForElement:defaultMenuItems:) method.

## Overview

These tags define common actions a user might want to take with elements in a page. You can use the tags to differentiate between the different types of menu items.

## Topics

### Constants

var WebMenuItemTagOpenLinkInNewWindow: Int

Open the link in a new window.

var WebMenuItemTagDownloadLinkToDisk: Int

Download the link to a disk.

var WebMenuItemTagCopyLinkToClipboard: Int

Copy the link to the clipboard.

var WebMenuItemTagOpenImageInNewWindow: Int

Open the image in a new window.

var WebMenuItemTagDownloadImageToDisk: Int

Download the image to disk.

var WebMenuItemTagCopyImageToClipboard: Int

Copy the image to the clipboard.

var WebMenuItemTagOpenFrameInNewWindow: Int

Open the frame in a new window.

var WebMenuItemTagCopy: Int

Copy the element to the clipboard.

var WebMenuItemTagGoBack: Int

Load the previous page.

var WebMenuItemTagGoForward: Int

Load the next page.

var WebMenuItemTagStop: Int

Stop loading the current page.

var WebMenuItemTagReload: Int

Reload the current page.

var WebMenuItemTagCut: Int

Cut the currently selected content.

var WebMenuItemTagPaste: Int

Paste the content on the clipboard onto the current selection.

var WebMenuItemTagSpellingGuess: Int

Suggest spellings for the misspelled word.

var WebMenuItemTagNoGuessesFound: Int

Indicate whether any suggested spellings for the misspelled word could be found.

var WebMenuItemTagIgnoreSpelling: Int

Ignore the misspelled word.

var WebMenuItemTagLearnSpelling: Int

Add the misspelled word to the user’s list of acceptable words.

var WebMenuItemTagOther: Int

Used when a tag for an item in the context menu can’t be determined.

var WebMenuItemTagSearchInSpotlight: Int

Search SpotLight for the current selection.

var WebMenuItemTagSearchWeb: Int

Search the web for the current selection.

var WebMenuItemTagLookUpInDictionary: Int

Look up the current selection in the Dictionary.

var WebMenuItemTagOpenWithDefaultApplication: Int

Open the current selection using the default application.

var WebMenuItemPDFActualSize: Int

Display a PDF document at its original size.

var WebMenuItemPDFZoomIn: Int

Scale up a PDF document.

var WebMenuItemPDFZoomOut: Int

Scale down a PDF document.

var WebMenuItemPDFAutoSize: Int

Display a PDF document at a user-specified size.

var WebMenuItemPDFSinglePage: Int

Display a PDF document one page at a time.

var WebMenuItemPDFFacingPages: Int

Display a PDF document two pages at a time.

var WebMenuItemPDFContinuous: Int

Display all pages in a PDF document continuously, using a vertical scroll bar, if necessary.

var WebMenuItemPDFNextPage: Int

Display the next page of a PDF document.

var WebMenuItemPDFPreviousPage: Int

Display the previous page of a PDF document.

## See Also

### Constants

struct WebDragDestinationAction

Actions that the destination object of a drag operation can perform.

Deprecated

struct WebDragSourceAction

Actions that the source object of a drag operation can perform.

Deprecated

