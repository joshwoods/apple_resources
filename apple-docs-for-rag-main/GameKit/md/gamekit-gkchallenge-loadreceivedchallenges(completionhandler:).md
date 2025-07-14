

- GameKit
- GKChallenge
-  loadReceivedChallenges(completionHandler:) 

Type Method

# loadReceivedChallenges(completionHandler:)

Loads the list of outstanding challenges.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
class func loadReceivedChallenges(completionHandler: (([GKChallenge]?, (any Error)?) -> Void)? = nil)
```

``` source
class func loadReceivedChallenges() async throws -> [GKChallenge]
```

## Parameters 

`completionHandler`  

The block that GameKit calls when it completes the request.

The block receives the following parameters:

`challenges`  
The challenges the local player issued.

`error`  
Describes an error if it occurs, or `nil` if the operation completes successfully.

