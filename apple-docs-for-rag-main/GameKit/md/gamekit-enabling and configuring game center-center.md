

- GameKit
-  Enabling and configuring Game Center 

Article

# Enabling and configuring Game Center

Enable Game Center in your Xcode project and configure features in App Store Connect.

## Overview

Before you can use the GameKit framework and access Game Center data, you need to enable Game Center. When you enable Game Center in your project, Xcode adds the Game Center entitlement to your App ID and adds the GameKit framework to your project. Then you can configure features that you use in your game, such as leaderboards and achievements, in App Store Connect.

For more information about the Game Center service, see Overview of Game Center.

### Enable Game Center

In Xcode, select the project in the main window, and in the project editor that appears on the right, select the target. Then click the Signing & Capabilities tab in the project editor and click the Library button (+) in the toolbar to open the Capabilities library. To enable Game Center, double-click the Game Center capability in the library or drag the capability from the library to the Signing & Capabilities pane.

For Mac targets, ensure that you enable both Incoming Connections and Outgoing Connections in the App Sandbox capability under Network.

### Configure Game Center features

If you don’t have an app record in App Store Connect, first create one so you can configure Game Center features while you develop your game. To create an app record in App Store Connect that matches your App ID in your developer account, see Add a new app in App Store Connect Help. To enable Game Center for versions of your app, see Enable your app version for Game Center. Then follow the steps in App Store Connect Help to configure leaderboards, achievements, and multiplayer games.

## See Also

### Essentials

Authenticating a player

Confirm player credentials and device capabilities and check for account restrictions.

Improving the player experience for games with large downloads

Provide ample content in your base installation and then use on-demand resources and the Background Assets API to handle additional content.

Game Center Entitlement

A Boolean value that indicates whether users of the app may see and compare achievements on a leaderboard, invite friends, and start multiplayer games.

