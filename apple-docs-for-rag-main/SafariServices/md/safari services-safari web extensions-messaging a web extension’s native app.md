

- Safari Services
- Safari web extensions
-  Messaging a Web Extension’s Native App 

Sample Code

# Messaging a Web Extension’s Native App

Communicate between your Safari web extension and its containing app.

Download

macOS 10.14+Xcode 12.0+

## Overview

Note

This sample code project is associated with WWDC20 session 10665: Meet Safari Web Extensions.

### Configure the Sample Code Project

Before you run the sample code project in Xcode:

1.  Open Safari and choose Develop \> Allow Unsigned Extensions.

2.  In the project settings in Xcode, select the Native Messaging Demo target.

3.  Click the Signing & Capabilities tab.

4.  For Signing Certificate, choose Sign to Run Locally. (Leave Team set to None.)

5.  Repeat steps 3 and 4 for the Native Messaging Demo Extension target.

## See Also

### Messaging

Messaging between the app and JavaScript in a Safari web extension

Communicate about events and share data between the containing app and JavaScript by using native messaging and app groups.

let SFExtensionMessageKey: String

A string the system uses as a key in a user info dictionary to identify a message.

let SFExtensionProfileKey: String

A string the system uses as a key in a user info dictionary to identify a profile identifier.

Messaging between a webpage and your Safari web extension

Configure your extension to enable messaging from webpages, and then update your extension to handle messages.

