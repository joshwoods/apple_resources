

- MusicKit
-  Using MusicKit to Integrate with Apple Music 

Sample Code

# Using MusicKit to Integrate with Apple Music

Find an album in Apple Music that corresponds to a CD in a user’s collection, and present the information for the album.

Download

iOS 15.0+iPadOS 15.0+Xcode 13.0+

## Overview

Note

This sample code project is associated with WWDC21 session 10294: Meet MusicKit for Swift.

### Configure the Sample Code Project

This sample code project must be run on a physical device.

Before you run the sample code project in Xcode, perform the following steps:

1.  In the Project navigator, select the project and click the *Signing & Capabilities* tab.

2.  Select your developer team from the *Team* menu.

3.  Choose a new bundle identifier for the `MusicAlbums` target, and enter it in the Bundle Identifier field. The bundle identifier within the project has an associated App ID, so you need a unique identifier to create your own App ID. Use a reverse-DNS format for your identifier, as Preparing your app for distribution describes.

4.  In Safari, visit the Certificates, Identifiers, and Profiles section of the developer web site.

5.  Select *Identifiers* and click the Add button to create a new App ID for `MusicAlbums`. Follow the steps until you reach the *Register an App ID* page.

6.  For the Bundle ID, select *Explicit*, and enter the bundle identifier from step 2.

7.  Click the *App Services* tab, and select the MusicKit checkbox.

8.  Complete the App ID creation process.

After creating your App ID, your Xcode project needs no additional configuration. The MusicKit App Service is a run-time service that automatically associates with your app’s bundle ID.

## See Also

### Essentials

Using Automatic Developer Token Generation for Apple Music API

Enable your app’s integration with the MusicKit App Service in the developer portal.

Explore more content with MusicKit

Track your outdoor runs with access to the Apple Music catalog, personal recommendations, and your own personal music library.

