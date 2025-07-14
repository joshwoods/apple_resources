

- App Store Connect API
- Game Center
- Expressions
-  Comparing app versions 

Article

# Comparing app versions

Return a Boolean value that indicates whether two match requests are from compatible app versions.

## Overview

Use the `areCompatibleAppVersions()` function in the expression of a matchmaking rule to determine if the version of the games that request matches are compatible. This function uses information you enter in App Store Connect — such as the bundle ID, platform, and version properties to determine compatibility. For more information, see Add multiplayer compatibility.

### Declaration

```
boolean areCompatibleAppVersions(object $request1, object $request2)
```

### Parameters

`request1`  
A match request to compare with `request2`.

`request2`  
A match request to compare with `request1`.

### Return value

`true`, if the game instances that request a match are compatible; otherwise, `false`.

