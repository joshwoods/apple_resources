

- SMS and Call Reporting
- SMS and MMS Message Filtering
-  Creating a Message Filter App Extension 

Article

# Creating a Message Filter App Extension

Create an app extension that helps identify unwanted messages.

## Overview

To create a Message Filter app extension, add a target that uses the Message Filter Extension template to the Xcode project for your containing app. The principal view controller in your app extension is a subclass of ILMessageFilterExtension that adopts the ILMessageFilterQueryHandling protocol.

If you have servers that can help your app extension determine how to handle a message, you must add the Associated Domains capability to your Xcode project and specify those domains. Then, you must set up shared credentials as described in Shared Web Credentials, substituting `messagefilter` for `webcredentials` throughout the steps. Lastly, you must specify the domains in your `Info.plist` file, which should look similar to the dictionary shown below.

```
```

