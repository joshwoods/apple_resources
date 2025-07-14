

- Safari Services
- Safari app extensions
-  Passing messages between Safari app extensions and injected scripts 

Article

# Passing messages between Safari app extensions and injected scripts

Communicate between your Safari app extension and injected scripts.

## Overview

The injected script and your Safari app extension live in different sandboxed worlds, each with specific limits on what it can access. You can’t call directly from the native code in your app extension to the injected script running in the browser. However, some sort of communication between the two is almost always desirable. For example, you may have a toolbar or contextual menu item that you want to use to affect web content.

The solution is to pass messages between the injected script and the app extension. The two runtime environments share a common format for message passing, and each provides an interface for sending and receiving messages.

The complete workflow appears below:

Within the scripting environment, you have access to the `window` and `document` objects for the browser content, as well as a `safari` object. The `safari` object is an instance of the `SafariAppExtensionNamespace` class. It provides details about your app extension and support for passing messages between your injected script and the app extension.

This table describes your app extension’s key properties:

| Property | Description |
|----|----|
| `extension` | A proxy for the app extension. Use it to retrieve information about your app extension and to pass messages to it. |
| `self` | A proxy for your injected script. Use it to install event listeners to respond to messages from your app extension. |

### Send messages to the app extension

Call `safari.extension.dispatchMessage.`

```
safari.extension.dispatchMessage("Hello World");

```

The parameter for dispatchMessage is a string that identifies the message you want to send. You create your own message names and decide what those messages mean for your app extension.

You can optionally send additional user data to accompany the message.

```
safari.extension.dispatchMessage("InterestingMessage",  { "key": "value" });
```

The user data must be a JavaScript object made up of keys and values that conform to the W3C standard for safe passing of structured data, such as Boolean objects, numeric values, strings, arrays, and so on.

For example, the following code sends an array in a message:

```
var myArray = ["a", "b", "c"];
safari.extension.dispatchMessage("passArray", { "key": myArray });
```

When the app extension receives the message, the system calls the extension handler’s messageReceived(withName:from:userInfo:) method. This method’s parameters include the message name, the page that sends the message, and, if part of the message, a user dictionary:

- Swift
- Objective-C

```
override func messageReceived(withName messageName: String, from page: SFSafariPage, userInfo: [String : AnyObject]!) {
    page.getPropertiesWithCompletionHandler { properties in
        NSLog("The extension received a message (\(messageName)) from a script injected into (\(properties?.url)) with userInfo (\(userInfo))")
    }
}
```

```
```

In Safari 17 and later, check whether the user is browsing with a profile if you need to limit any extension logic to the profile, such as fetching or storing data. To do that, implement the beginRequest(with:) method.

```
- (void)beginRequestWithExtensionContext:(NSExtensionContext *)context {
    NSExtensionItem *item = context.inputItems.firstObject;
    NSDictionary *userInfo = item.userInfo;
    NSUUID *profileIdentifier = userInfo[SFExtensionProfileKey];

    if (profileIdentifier != nil) {
        // Remember profile identifier for future method calls.
    } else {
        // Handle normal browsing. 
    }
}
```

Then, get the profile identifier from the `context.inputItems` dictionary using SFExtensionProfileKey as the key. Use the profile identifier for any profile-specific logic.

### Send messages to the injected script

When the app extension needs to send a message to an injected script, it calls the dispatchMessageToScript(withName:userInfo:) method on the target page.

- Swift
- Objective-C

```
override func messageReceived(withName messageName: String, from page: SFSafariPage, userInfo: [String : AnyObject]!) {
    page.dispatchMessageToScript(withName: "simpleMessage", userInfo: nil)
    page.dispatchMessageToScript(withName: "complexMessage", userInfo: ["myKey": "myValue"])
}
```

```
```

The message is a packaged event with a type of `message`. To respond to the message, the injected script registers an event listener for message events using `safari.self.addEventListener.`

```
safari.self.addEventListener("message", handleMessage);

```

The event that passes into the event handler is a SafariExtensionMessageEvent object. Its `name` property identifies the message, and its `message` property contains the dictionary of user data.

```
function handleMessage(event) {
    console.log(event.name);
    console.log(event.message);
}
```

## See Also

### Related Documentation

SafariAppExtension

A class that represents your extension in a content script.

SafariAppExtensionPage

A class that represents a web content area.

SafariEventTarget

A base class for event dispatching.

SafariExtensionMessageEvent

A class that represents a message between the web content area and an outside script.

### Injected style sheets and scripts

Using injected style sheets and scripts

Learn how you can affect the appearance or behavior of a webpage by using injected style sheets and scripts.

Injecting a script into a webpage

Inject a script that you write for a Safari app extension into a webpage.

Injecting CSS style sheets into a webpage

Add to or override styles by injecting CSS style sheets into webpages.

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

