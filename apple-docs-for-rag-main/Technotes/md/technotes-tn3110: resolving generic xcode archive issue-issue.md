

- Technotes
-  TN3110: Resolving generic Xcode archive issue 

Article

# TN3110: Resolving generic Xcode archive issue

Identify common configurations that cause a generic Xcode archive.

## Overview

The Archives organizer reports your archive as an *app archive* if it contains a single top-level app and a *generic Xcode archive*, otherwise.  You can validate and distribute an app archive. A generic archive, which may contain unexpected items such as header files, static libraries, or frameworks, can’t be validated nor distributed.

## Ensure the Skip Install build setting is properly configured

The Skip Install (SKIP_INSTALL) build setting determines whether to install built products within the archive.

When enabled for an app, Xcode doesn’t install the app within the archive. The produced archive doesn’t contain the single top-level app as expected. To generate an app archive, confirm that Skip Install is disabled for your app. 

When disabled for an app’s dependencies such as frameworks, Xcode adds these dependencies to the app’s archive. The produced archive contains multiple folders rather than the expected single top-level app. To generate an app archive, confirm that Skip Install is enabled for all your app’s dependencies. 

## Use a Copy Files build phase

If your app links against static libraries, confirm that they all use a Copy files build phase to export their header files. The produced app archive contains header files when static libraries use a Headers build phase to export these files.

## Ensure the Installation Directory build setting is properly configured

The Installation Directory (INSTALL_PATH) build setting specifies the directory where to install built products. It takes default values according to the product being built. To generate an app archive, confirm that Installation Directory is set to the default value such as `$(LOCAL_APPS_DIR)` for apps.

## Revision History

- **2022-02-08** First published.

## See Also

### Latest

TN3182: Adding privacy tracking keys to your privacy manifest

Declare the tracking domains you use in your app or third-party SDK in a privacy manifest.

TN3183: Adding required reason API entries to your privacy manifest

Declare the APIs that can potentially fingerprint devices in your app or third-party SDK in a privacy manifest.

TN3184: Adding data collection details to your privacy manifest

Declare the data your app or third-party SDK collects in a privacy manifest.

TN3181: Debugging an invalid privacy manifest

Identify common configurations that cause unsuccessful privacy manifest validation with the App Store.

TN3180: Reverting to App Store Server Notifications V1

Migrate from version 2 to version 1 of App Store Server Notifications using the Modify an App endpoint.

TN3179: Understanding local network privacy

Learn how local network privacy affects your software.

TN3178: Checking for and resolving build UUID problems

Ensure that every Mach-O image has a UUID, and that every distinct Mach-O image has its own unique UUID.

TN3177: Understanding alternate audio track groups in movie files

Learn how alternate groups collect audio tracks, and how to choose which audio track to use in your app.

TN3111: iOS Wi-Fi API overview

Explore the various Wi-Fi APIs available on iOS and their expected use cases.

TN3176: Troubleshooting Apple Pay payment processing issues

Diagnose errors that occur when processing Apple Pay payments, identify common causes, and explore potential solutions.

TN3175: Diagnosing issues with displaying the Apple Pay button on your website

Diagnose common errors received while displaying the Apple Pay button on your website by identifying the underlying causes, and explore potential solutions.

TN3174: Diagnosing issues with the Apple Pay payment sheet on your website

Diagnose errors received while presenting the Apple Pay payment sheet on your website by identifying the underlying causes of common errors and explore their potential solutions.

TN3173: Troubleshooting issues with your Apple Pay merchant identifier configuration

Diagnose errors due to invalid Apple Pay merchant identifier configurations by identifying the underlying causes of common errors and explore their potential solutions.

TN3168: Making your App Clip available in the App Store

Learn how to configure your App Clip to prevent it from being unavailable in the App Store.

TN3124: Debugging coordinate space issues

Learn techniques to help debug any coordinate space issue.

