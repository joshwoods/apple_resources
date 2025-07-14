

- CKTool JS
-  Team 

Structure

# Team

Details of a developer team.

CKTool JS 1.2.15+

``` source
dictionary Team {
 string teamId;
 string teamName;
 string? teamType;
};
```

## Overview

You can find your team details in the Membership tab of the Apple Developer portal at `https://developer.apple.com`.

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { Team } from "@apple/cktool.database";
```

## Topics

### Instance Properties

teamId

Unique identifier of the developer team.

teamName

Name of the developer team.

teamType

Type of the developer team.

## See Also

### User and Team

getSessionUser

Returns details for the user in current session.

getTeams

Fetches a list of teams the current user is in.

TeamsResponse

Response object for a list of teams.

