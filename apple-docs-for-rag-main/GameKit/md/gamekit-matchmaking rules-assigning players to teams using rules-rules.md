

- GameKit
- Matchmaking rules
-  Assigning players to teams using rules 

Article

# Assigning players to teams using rules

Set criteria for assigning players to teams in your game using matchmaking rules.

## Overview

If your game has teams, add team rules to balance the assignment of players to teams that makes gameplay more fair and enjoyable for the players. Team rules create constraints on adding players to teams.

Game Center applies the team rules to match requests in the queue after applying other compatible, distance, and match rules. Game Center applies the team rules to candidate teams from combinations of compatible match requests.

Before you begin adding team rules:

- Create a rule set to contain the team rules using the Create a rule set endpoint.

- Add compatibility and distance rules that filter the match requests using the Create a rule endpoint.

- Add match rules, such as skill-level rules, that apply to compatible requests.

For more information on creating the other types of rules, see Letting players join matches using party codes and Finding players with similar skill levels.

### Add teams to the rule set

Create two or more teams to compete in your game using the Create a team endpoint.

In the attributes property, pass the minimum and maximum players, and a name of the team. In the relationships property, pass the rule set `id` that the Create a rule set endpoint returns in the response.

```
```

Create one or more other teams to compete with the first team using a different name and add them to the same rule set:

```
```

### Add team rules to the rule set

You can add one or more team rules to your rule set depending on how many constraints you want to add to the team assignments. For example, if your matches have a variable number of team members, you can create a team rule that keeps the sizes of the teams balanced. You can also balance the teams by skill level and ensure that invited players are on the same team.

To create a team rule, set the rule’s type field to `TEAM` and the `teams` array becomes available to use in expressions. The `teams` array contains `Team` objects that represent the teams in the rule set. A team has a `players` property that contains `Player` objects that represent the players assigned to the team.

Write an expression that returns true when the size of the teams are the same using expression functions, the `teams` array, and the `players` property.

```
```

Pass the rule type, the expression, and the rule set, along with other settings, to the Create a rule endpoint.

```
```

In team rule expressions, the Player object has a `requestName` field that is an identifier for the associated match request. For more information on the Team and Player objects you use in team rules, see Expressions in App Store Connect API.

### Create match requests that assign players to teams

In your code, create a GKMatchRequest object that initiates a team game. Set the queueName property to the reference name of the queue that contains your team rules.

```
// Create a match request.
let request = GKMatchRequest()

// Set the matchmaking rules queue name.
request.queueName = "com.example.mygame.TeamBasedQueue"
```

If you add a rule to balance the teams by skill level, add the local player’s skill to the properties property:

```
// Set properties to the game-specific keys you use in the rules.
let skill = localPlayerData.skill
request.properties = [ "skill": skill]
```

Game Center finds all compatible players and assigns them to teams.

### Get team assignments when players accept invitations

When all the players accept their invitations, GameKit invokes the `GKMatchmakerViewControllerDelegate` matchmakerViewController(_:didFind:) method in the app instances for all players in the game, including the player who sent the invitations.

```
func matchmakerViewController(_ viewController: GKMatchmakerViewController,
                                  didFind match: GKMatch) {
    // Dismiss the view controller.
    viewController.dismiss(animated: true, completion: nil)

    // Set the match delegate.
    match.delegate = myGame

    // Start the game with the players in the match.
}
```

Before your implementation of this delegate method starts the game, you can get all the team assignments from the GKMatch object. Use the players property to get the players that accepted the invitation, including the player that initiated the match. Then use the ``` GKMatch.``playersProperties ``` to get the game-specific properties for each player, such as the `skill` property, including the team assignment. If you add team rules to your rule set, use the `gc` and `team` keys to get the name of the player’s team that you previously configured using the Create a team endpoint.

```
// Get the local player's team assignment.
properties = match.properties
team = properties["gc"]["team"]
```

## See Also

### Rules

Letting players join matches using party codes

Add a rule that lets players invite players and join matches using a shared party code.

Finding players with similar skill levels

Add a rule to find players in a range of skill levels to balance competitive gameplay.

Creating matchmaking rules for backward compatibility

Add matchmaking rules that support previous classic matchmaking versions of your game.

