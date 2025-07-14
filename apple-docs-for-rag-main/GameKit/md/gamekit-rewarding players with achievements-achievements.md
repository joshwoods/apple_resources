

- GameKit
-  Rewarding players with achievements 

Article

# Rewarding players with achievements

Use achievements to motivate players and engage them more in your game.

## Overview

An *achievement* is a collectible item that a player receives as a reward for successfully reaching a particular goal in your game. Achievements provide players an additional way of engaging with your game, tracking gameplay progress, and sharing that progress with friends. You define the achievements available to players in your game, and Game Center saves the progress players make toward earning them. Players can view your game achievements and track their progress in the dashboard.

Your game can have a maximum of 100 achievements, 100 points per achievement, and 1000 points total for all achievements. To keep players engaged, you can progressively add achievements to each version of your game until you reach the limit.

For design guidance, see Human Interface Guidelines > Technologies > Game Center > Achievements.

### Configure achievements

Before you can access achievements in your code, you can configure them in Xcode and sync the configuration updates you make with App Store Connect. Begin configuring achievements by creating a GameKit configuration file. In Xcode, choose File \> New \> File from Template. Select GameKit File, and click Next. In the sheet that appears, enter a name for the configuration and click Create.

If you’ve already configured achievements in App Store Connect, click More (…) at the bottom of the left column. Then choose Pull from App Store Connect. Select the bundle ID or Game Center group for your game from the list, and click pull. Resource details appear in the editor on the right.

To create a new achievement, click Add (+) at the bottom of the left column, and choose Achievement. When you create an achievement, you specify details like how many points the players earn for it, and whether they can earn the achievement more than once.

Tip

Reorganize the list of leaderboards and leaderboard sets that Xcode displays in the order you want Game Center to present them.

You also localize the user-facing text and assets in each language and region you support, and specify whether to hide the achievement from players before they reach a goal in your game. If you don’t hide the achievement, Game Center shows it immediately in the locked state. Players can browse all the achievements in your game, including locked achievements, to learn more about them.

If you add an achievement to an unreleased version of your game or sign the game with a development certificate, Game Center annotates the achievement with a prerelease indicator. For example, if you run your game in Xcode, a prerelease indicator appears next to the achievement name and a message appears in the detail view. To change an achievement’s app version, see Add achievements to an app version.

Note

If you’ve already pushed your configuration changes to App Store Connect, removing a leaderboard or leaderboard set from the local configuration file doesn’t remove the leaderboard or leaderboard set from App Store Connect.

To learn more about the information you enter in App Store Connect, see Achievement properties.

### Test achievements by using the Progress Manager

Before you begin testing your GameKit configuration, you need to enable Debug Mode. In Xcode, choose Product \> Scheme \> Edit Scheme. From the Run configuration, select Options and toggle Enable Debug Mode.

To begin testing your achievement configuration, open the game Progress Manager. In Xcode, choose Debug \> GameKit \> Manage Game Progress. From the top left of the window that appears, select the physical device you use for testing, and the project you want to debug. The test data stays local to your machine and doesn’t rely on App Store Connect to test.

After selecting the device and app, choose the achievement you want to test. Update the progress for an achievement in the detail panel on the right. When the progress updates, the system sends an update to your app so you can verify that the achievement changes.

If you want to reset the progress for your achievements and leaderboards, click the reset button at the top of the Progress Manager. You can’t access previous occurrences of achievements and leaderboards after resetting the Progress Manager.

### Get the object that represents the achievement

To start or continue reporting progress toward an achievement, you need a GKAchievement object that represents the achievement.

Load the in-progress achievements for the player using the loadAchievements(completionHandler:) method. Use the identifier you enter in Xcode to find the corresponding `GKAchievement` object in the array that GameKit passes to the completion handler.

```
// Load the player's active achievements.
let achievements = try await GKAchievement.loadAchievements()
let achievementID = "101"

// Find an existing achievement.
var achievement = achievements.first(where: { $0.identifier == achievementID })

// Otherwise, create a new achievement.
if achievement == nil {
    achievement = GKAchievement(identifier: achievementID)
}
```

If the achievement isn’t in the array, your game hasn’t reported any progress toward this achievement for this player yet, and the dashboard shows it in the locked state. You must create a new GKAchievement object using the identifier from App Store Connect. For the local player, use the init(identifier:) method to create the GKAchievement object. For another player, when ending a turn-based match, use the init(identifier:player:) method.

### Report the player’s progress

Initially, the percentage complete is `0` and the dashboard shows the achievement in the locked state. As the player progresses toward earning an achievement, you report the percentage the player completes for the achievement to Game Center.

Set the achievement’s percentComplete property to a value between `0` and `100`. For example, increase the percentage complete by 10%.

```
achievement.percentComplete = achievement.percentComplete + 10.0
```

Then report the progress to Game Center by passing the achievement in an array to the report(_:withCompletionHandler:) method.

```
// Create an array containing the achievement.
let achievementsToReport: [GKAchievement] = [achievement]

// Report the progress to Game Center.
try await GKAchievement.report(achievementsToReport)
```

When reporting a percentage greater than `0` and less than `100`, the dashboard shows the achievement as in-progress. When you report that the player completes the achievement 100%, the dashboard shows the image for the achievement, and Game Center adds it to the player’s completed achievements.

GameKit also displays a banner notifying the player when they complete an achievement. If you want to display your own interface, set the showsCompletionBanner property to false before reporting the player’s progress so the default banner doesn’t appear.

You can also hide an achievement in Xcode when you configure it, and not report on the progress until the player completes it. For example, use a hidden achievement if an achievement description reveals aspects of your game’s plot, or if you want to surprise the player with awards.

If the player completes all achievements in your game or if you want to clear all progress the local player makes toward all their achievements, you can reset them using the resetAchievements(completionHandler:) class method.

### Show achievements to players

Players can view their achievements in the dashboard, which provides a familiar and consistent experience for users. You can add the access point to your game so players can open the dashboard and navigate to their achievements. The access point displays achievements in the highlights, and on the dashboard when the player opens it. You can also display the dashboard in the state that shows the achievements so players can drill down and navigate to their other Game Center data.

If you want to display the data directly in your interface, you can load details of all the achievements, including their identifiers and artwork, using the loadAchievementDescriptions(completionHandler:) class method. GameKit returns the localized achievement titles and descriptions, which you provide when you configure the achievements in App Store Connect. To load the artwork for an achievement, use the loadImage(completionHandler:) method.

## See Also

### Related Documentation

Adding an access point to your game

Provide your users a convenient connection to the Game Center dashboard.

Displaying the Game Center dashboard

Provide an interface for players to navigate to their Game Center data from your game.

### Achievements

class GKAchievement

An achievement you can award a player as they make progress toward and reach a goal in your game.

class GKAchievementDescription

An object containing the text and artwork used to present an achievement to a player.

