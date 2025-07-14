

- WebKit
- Deprecated Symbols
- Setting Up a Web View (Legacy)
- WebView
-  Element Dictionary Keys 

API Collection

# Element Dictionary Keys

Predefined keys used to access an element dictionary.

## Overview

These constants represent predefined keys used to access an element dictionary. An element dictionary is an NSDictionary representation of an HTML element, as in a clicked or selected element. Some methods in the WebPolicyDelegate informal protocol have an element dictionary argument. The descriptions below describe the dictionary value for the key.

## Topics

### Constants

let WebElementDOMNodeKey: String

The DOMNode for this element.

Deprecated

let WebElementFrameKey: String

The WebFrame object associated with this element.

Deprecated

let WebElementImageAltStringKey: String

An NSString of the ALT attribute of an image element.

Deprecated

let WebElementImageKey: String

An NSImage representing an image element.

Deprecated

let WebElementImageRectKey: String

An NSValue containing an NSRect, the size of an image element.

Deprecated

let WebElementImageURLKey: String

An NSURL containing the location of an image element.

Deprecated

let WebElementIsSelectedKey: String

An NSNumber used as a BOOL value to indicate whether a text element is selected or not. Zero value indicates false, true otherwise.

Deprecated

let WebElementLinkURLKey: String

An NSURL containing the location of a link if the element is within an anchor.

Deprecated

let WebElementLinkTargetFrameKey: String

The WebFrame object associated with the target of the anchor.

Deprecated

let WebElementLinkTitleKey: String

An NSString containing the title of an anchor.

Deprecated

let WebElementLinkLabelKey: String

An NSString containing the text within an anchor.

Deprecated

