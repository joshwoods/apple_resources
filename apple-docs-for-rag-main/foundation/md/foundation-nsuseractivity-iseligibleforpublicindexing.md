

- Foundation
- NSUserActivity
-  isEligibleForPublicIndexing 

Instance Property

# isEligibleForPublicIndexing

A Boolean value that indicates whether the activity can be publicly accessed by all iOS users.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var isEligibleForPublicIndexing: Bool { get set }
```

## Mentioned in 

Creating a user activity object

## Discussion

The default value of this property is false, which indicates that the activity object contains private or sensitive information or that the activity isn’t useful to other users. When the value of this property is true, the system identifies this activity as one that can be shared publicly. When you make an activity public, the system indexes the values in the requiredUserInfoKeys or webpageURL properties, and you must provide a value for one of those properties.

Identifying an activity as public confers an advantage when you also add web markup to the content on your related website. Specifically, when users engage with your app’s public activities in search results, it indicates to Apple that public information on your website is popular, which can help increase your ranking and potentially lead to expanded indexing of your website’s content.

## See Also

### Specifying the activity’s eligibility

var isEligibleForHandoff: Bool

A Boolean value that indicates whether the activity can be continued on another device using Handoff.

var isEligibleForSearch: Bool

A Boolean value that indicates whether the activity should be added to the on-device index.

var expirationDate: Date?

The date after which the activity is no longer eligible for Handoff or indexing.

