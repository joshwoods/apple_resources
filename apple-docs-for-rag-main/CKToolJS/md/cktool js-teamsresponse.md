

- CKTool JS
-  TeamsResponse 

Structure

# TeamsResponse

Response object for a list of teams.

CKTool JS 1.2.15+

``` source
dictionary TeamsResponse {
 Team[] teams;
 string? recentTeamId;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { TeamsResponse } from "@apple/cktool.database";
```

## Topics

### Instance Properties

recentTeamId

Most recently used developer `teamId`.

teams

The array of teams fetched.

## See Also

### User and Team

getSessionUser

Returns details for the user in current session.

getTeams

Fetches a list of teams the current user is in.

Team

Details of a developer team.

