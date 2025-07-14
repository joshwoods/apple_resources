

- App Store Connect API
- Game Center
- Expressions
-  Keeping invited players on the same team 

Article

# Keeping invited players on the same team

Return a Boolean value that indicates whether players in the same match requests are on the same team.

### Declaration

```
boolean hasInvitedPlayersOnSameTeam(array[object] $teams, array[object] $players)
```

### Parameters

`teams`  
The teams in the rule set. Pass the `teams` array that’s available in team rule expressions.

`players`  
The players that the rule applies to. Pass the `players` array that’s available in team rule expressions.

### Return value

`true` if the players in the same match requests are on the same team; otherwise, `false`. The players in a match request include the local player and any recipients or other players that the local player invites.

