

- Technotes
-  TN3154: Adopting SwiftUI navigation split view 

Article

# TN3154: Adopting SwiftUI navigation split view

Use navigation split view to enable two and three column navigation in your SwiftUI app while maintaining compatibility with earlier OS versions.

## Overview

NavigationSplitView is a view that presents views in two or three columns, where selections in leading columns control presentations in subsequent columns. The Navigation split view API is available on iOS 16, macOS 13, tvOS 16, watchOS 9 and visionOS 1.

Transition from the deprecated NavigationView API if your app has a minimum deployment target of at least iOS 16, macOS 13, tvOS 16, watchOS 9 or visionOS 1. For more information, see Migrating to new navigation types.

This document describes how using a custom wrapper makes it easier to adopt `NavigationSplitView` and ensures your app remains compatible with the deprecated `NavigationView`, without increasing the app deployment target.

## Using API availability check to provide backward compatibility using a custom wrapper

Use the `#available()` keyword to execute code conditionally based on required platform and version. This allows your app use `NavigationSplitView` if the specified OS versions are iOS 16, macOS 13, tvOS 16, watchOS 9 or visionOS 1 while supporting `NavigationView` for earlier OS versions.

To ensure backward compatibility on earlier versions of iOS, macOS, tvOS and watchOS, create and use a custom wrapper view that conditionally uses either `NavigationSplitView` or `NavigationView` depending on the availability of the API. For apps that use one column navigation view, consider using NavigationStack.

```
struct NavigationSplitViewWrapper: View where Sidebar: View, Content: View, Detail: View {
    private var sidebar: Sidebar
    private var content: Content
    private var detail: Detail

    init(
        @ViewBuilder sidebar: () -> Sidebar,
        @ViewBuilder content: () -> Content,
        @ViewBuilder detail:  () -> Detail
    ) {
        self.sidebar = sidebar()
        self.content = content()
        self.detail = detail()
    }

    var body: some View {
        if #available(iOS 16, macOS 13, tvOS 16, watchOS 9, visionOS 1, *) {
            // Use the latest API available
            NavigationSplitView {
                sidebar
            } content: {
                content
            } detail: {
                detail
            }
        } else {
            // Alternative code for earlier versions of OS.
            NavigationView {
                // The first column is the sidebar.
                sidebar

                // Initial content of the second column.
                content

                // Initial content for the third column.
                detail
            }
            .navigationViewStyle(.columns)
        }
    }
}
```

Note

Navigation split view collapses all of its columns into a stack and shows the last column that displays useful information for compact size classes, such as on iPhone or in iPad’s Slide Over mode. It also collapses all of its columns into a stack on Apple Watch and Apple TV, regardless of the size class.

## Revision History

- **2023-08-29** First published.

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

