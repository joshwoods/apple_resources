

- App Clips
-  Creating App Clip Codes 

Article

# Creating App Clip Codes

Help users discover your App Clip by using an NFC-integrated or scan-only App Clip Code.

## Overview

An App Clip Code is immediately recognizable to users and lets them know an App Clip is available. The App Clip Code offers a fast and secure launch experience for your App Clip that users trust.

The visual design of an App Clip Code encodes your App Clip’s *invocation URL*. Optionally, you can embed an NFC tag that also encodes the invocation URL. An App Clip Code with an embedded NFC tag is called an *NFC-integrated* App Clip Code, while a code without an NFC tag is called a *scan-only* App Clip Code.

The image at the center of an App Clip Code icon lets users know how to interact with the code. If they discover an NFC-integrated App Clip Code, they hold their device close to the code or scan it with the NFC Tag Reader in Control Center to launch your App Clip. They can also scan an NFC-integrated App Clip Code with the Camera app or the Code Scanner in Control Center. If they discover a scan-only App Clip Code, they scan it with the Camera or the Code Scanner in Control Center to launch your App Clip.

In addition to providing a great launch experience for your App Clip, you can also use an App Clip Code to offer a context-aware augmented reality experience. For more information, see Interacting with App Clip Codes in AR.

Note

Scanning App Clip Codes requires a device that runs iOS 14.3 or later.

Creating an App Clip Code requires the following tasks:

1.  Choosing an invocation URL and configuring an *advanced App Clip experience* in App Store Connect. To learn more, see Configuring the launch experience of your App Clip.

2.  Choosing the type (scan-only or NFC-integrated), colors, and design of your App Clip Code. For design guidance, see Human Interface Guidelines > App Clips > App Clip Codes.

3.  Generating App Clip Codes with App Store Connect or with the App Clip Code Generator command-line tool. For more information, see Pick a tool to create App Clip Codes below.

4.  Printing App Clip Codes yourself or with the help of a professional printing service — for example, RR Donnelley. For printing guidance, see Human Interface Guidelines > App Clips > Printing Guidelines and Preparing multiple App Clip Codes for production.

For more information, see Encoding a URL in an App Clip Code.

### Pick a tool to create App Clip Codes

App Clip Codes always use the design Apple provides to ensure users instantly recognize them. You can create an App Clip Code by selecting an advanced App Clip experience in App Store Connect or by installing the App Clip Code Generator command-line tool. Both have similar features and it’s up to you to pick the tool that best fits your needs.

Consider using App Store Connect if:

- You’ve already created an advanced App Clip experience in App Store Connect.

- You prefer an instantaneous preview while you experiment with colors.

- You’re comfortable using a tool that offers a more visual interface compared to a command-line tool.

Consider using the App Clip Code Generator command-line tool if:

- You haven’t created an advanced App Clip experience in App Store Connect — for example, during development of your App Clip.

- You need to create a lot of App Clip Codes and want to automate their creation with a script.

- You’re comfortable using a command-line tool.

For more information, see Creating App Clip Codes with App Store Connect and Creating App Clip Codes with the App Clip Code Generator.

Note

You must be enrolled in the Apple Developer Program before you can download the App Clip Code Generator. For information about the Apple Developer Program, see How the Program Works.

## See Also

### App Clip Codes

Preparing multiple App Clip Codes for production

Prepare your App Clip Codes to send to a professional printing service.

Interacting with App Clip Codes in AR

Display content and provide services in an AR experience with App Clip Codes.

