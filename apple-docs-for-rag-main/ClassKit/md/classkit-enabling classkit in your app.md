

- ClassKit
-  Enabling ClassKit in your app 

# Enabling ClassKit in your app

Prepare your app and your development environment to adopt ClassKit.

## Overview

Adopting ClassKit allows your app to participate in a virtual classroom that spans many devices communicating through iCloud. To participate in this educational ecosystem, first enable the ClassKit capability. Then, to test your app’s interaction with this ecosystem, install Apple’s Schoolwork app on your development devices and simulate iCloud interaction by running in development mode.

### Enable the ClassKit Capability

To gain access to the virtual classroom environment, enable the ClassKit capability for your app in Xcode.

When you enable the ClassKit capability, Xcode automatically adds the ClassKit Environment Entitlement to your entitlements file. It also adds the corresponding feature to your App ID. See Add a Capability in Xcode help for more information about enabling capabilities.

### Install the Schoolwork app on your devices

The Schoolwork app provides the interface that teachers use to see what content your app offers, create assignments based on that content, and monitor student progress through those assignments. Students use the same app to receive assignments, and link directly to content in your app. Schoolwork provides both of these experiences by changing its behavior according to the role of the logged in user. For more information about user roles, see About ClassKit and user roles.

To test your app’s ClassKit adoption, you install Schoolwork on your own development devices. This lets you validate the data your app sends to ClassKit. It also lets you experience what teachers and students see when they use your app in an educational environment.

To get Schoolwork, download it from the App Store.

Note

You can’t test ClassKit behavior in Simulator because Schoolwork isn’t available in that environment.

### Use development mode to test locally

When you distribute your ClassKit enabled app through the App Store, it runs in *production mode*. In this mode, assigments made by teachers propagate to students’ devices, and progress returns to the teacher’s device through iCloud. But during development, you might not have access to a classroom full of managed devices. So you test in *development mode*, storing all data locally on a single device, switching between teacher and student roles as needed. Xcode automatically handles the mode selection for you, but you control the role (student or teacher) in development mode, as described in Testing your ClassKit app during development.

## Topics

### Development mode

Testing your ClassKit app during development

Use development mode to test your app without a Managed Apple ID.

### User roles

About ClassKit and user roles

Understand how ClassKit interacts with different kinds of users.

## See Also

### Essentials

ClassKit Environment Entitlement

The ClassKit development or production environment for an education app that works with the Schoolwork app.

Incorporating ClassKit into an Educational App

Walk through the process of setting up assignments and recording student progress.

class CLSDataStore

A container for all the ClassKit data in your app.

