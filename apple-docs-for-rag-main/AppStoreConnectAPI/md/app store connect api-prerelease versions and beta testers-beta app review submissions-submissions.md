

- App Store Connect API
- Prerelease Versions and Beta Testers
-  Beta App Review Submissions 

API Collection

# Beta App Review Submissions

The submissions of builds for beta app review, including the status of submissions.

## Overview

A `betaAppReviewSubmissions` resource represents Apple’s review of a build before its distribution through TestFlight. Create a beta app review submission when you are ready to submit a build. App Store Connect validates the beta app review submission to ensure it includes necessary information such as `appEncryptionDeclarations`, `betaAppReviewDetails`, and so on, and submits the build to the review team.

API users can get the `betaAppReviewSubmissions` to see if the build has been accepted or rejected.

## Topics

### Submitting an App for Beta Review

Submit an App for Beta Review

Submit an app for beta app review to allow external testing.

### Getting Beta App Review Submissions Info

List Beta App Review Submissions

Find and list beta app review submissions for all builds.

Read Beta App Review Submission Information

Get a specific beta app review submission.

### Getting Build Information

Read the Build Information of a Beta App Review Submission

Get the build information for a specific beta app review submission.

### Objects and Data Types

object BetaAppReviewSubmission

The data structure that represents a Beta App Review Submissions resource.

object BetaAppReviewSubmissionCreateRequest

The request body you use to create a Beta App Review Submission.

object BetaAppReviewSubmissionResponse

A response that contains a single Beta App Review Submissions resource.

object BetaAppReviewSubmissionWithoutIncludesResponse

object BetaAppReviewSubmissionsResponse

A response that contains a list of Beta App Review Submission resources.

type BetaReviewState

String that indicates the review state of a beta app.

## See Also

### Beta App Review Submissions

Beta App Review Detail

Information about your app required for beta app review.

