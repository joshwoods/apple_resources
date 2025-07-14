

- App Store Connect API
-  BetaAppReviewSubmission 

Object

# BetaAppReviewSubmission

The data structure that represents a Beta App Review Submissions resource.

App Store Connect API 1.0+

``` source
object BetaAppReviewSubmission
```

## Properties

`attributes`

BetaAppReviewSubmission.Attributes

The resource’s attributes.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`links`

ResourceLinks

Navigational links that include the self-link.

`relationships`

BetaAppReviewSubmission.Relationships

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `betaAppReviewSubmissions`

## Topics

### Objects

object BetaAppReviewSubmission.Attributes

Attributes that describe a Beta App Review Submissions resource.

object BetaAppReviewSubmission.Relationships

The relationships you included in the request and those on which you can operate.

## See Also

### Objects and Data Types

object BetaAppReviewSubmissionCreateRequest

The request body you use to create a Beta App Review Submission.

object BetaAppReviewSubmissionResponse

A response that contains a single Beta App Review Submissions resource.

object BetaAppReviewSubmissionWithoutIncludesResponse

object BetaAppReviewSubmissionsResponse

A response that contains a list of Beta App Review Submission resources.

type BetaReviewState

String that indicates the review state of a beta app.

