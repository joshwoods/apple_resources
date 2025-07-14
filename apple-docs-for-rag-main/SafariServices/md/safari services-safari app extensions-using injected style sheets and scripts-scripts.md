

- Safari Services
- Safari app extensions
-  Using injected style sheets and scripts 

Article

# Using injected style sheets and scripts

Learn how you can affect the appearance or behavior of a webpage by using injected style sheets and scripts.

## Overview

To add or override styles and behaviors in a webpage, you write style sheets and scripts that you then inject into your webpage to read and modify its content.

### Add injected style sheets

Injected style sheets function like user style sheets, as defined by the W3C. The system adds styles in the following order:

1.  Your Safari app extension styles

2.  The webpage author’s styles

3.  The webpage author’s styles that are declared as `!important`

4.  Your Safari app extension styles that are declared as `!important`

At each stage, a new definition overrides any previous definition. The system adds style properties in your injected style sheets to existing page style properties, but your styles don’t override existing page styles unless you declare the new ones as `!important`.

For example, adding the following styles overrides a website using color text on a color background, and sets it to black text on a white background for a particular element:

```
span.anElement {
    color:black;
    background:white;
}
```

### Add injected scripts

You can inject `.js` files (text files that contain JavaScript functions and commands) into a webpage. The scripts in these files have access to the DOM of the webpages you inject them into. They have the same access privileges as scripts that execute from a webpage’s host. Injected scripts load each time a webpage loads, so keep them lightweight.

The system injects scripts into the top-level page and any subpages with HTML sources, such as iframes. Don’t assume that there’s only one instance of your script per browser tab. If you don’t want your injected script to execute inside iframes, preface your high-level functions with a test, as the following example shows:

```
if (window.top === window) {
    // The containing frame is the top-level frame, not an iframe.
    // All non-iframe code goes before the closing brace.
}
```

Injected scripts have an implied namespace — you don’t have to worry about your variable or function names conflicting with those of the website author, nor can a website author call functions in your extension. In other words, injected scripts and scripts that you include in the webpage run in isolated worlds, with no access to each other’s functions or data.

## See Also

### Injected style sheets and scripts

Injecting a script into a webpage

Inject a script that you write for a Safari app extension into a webpage.

Injecting CSS style sheets into a webpage

Add to or override styles by injecting CSS style sheets into webpages.

Passing messages between Safari app extensions and injected scripts

Communicate between your Safari app extension and injected scripts.

class SFSafariExtensionHandler

A base class that you subclass to handle events in your Safari app extension.

class SFSafariExtensionManager

A class that your app uses to find out the current state of a Safari app extension.

class SFSafariExtensionState

The state of a Safari app extension.

class SFSafariPageProperties

An object that captures information about a webpage.

protocol SFSafariExtensionHandling

A protocol for implementing event handling in a Safari app extension.

let SFExtensionProfileKey: String

A string the system uses as a key in a user info dictionary to identify a profile identifier.

