

- App Store Connect API
- CiBuildRun
-  CiBuildRun.Attributes 

Object

# CiBuildRun.Attributes

The attributes that describe a Build Runs resource.

App Store Connect API 1.5+

``` source
object CiBuildRun.Attributes
```

## Properties

`cancelReason`

`string`

A string that indicates the reason for a canceled build.

Possible Values: `AUTOMATICALLY_BY_NEWER_BUILD, MANUALLY_BY_USER`

`completionStatus`

CiCompletionStatus

A string that indicates the status of a completed build.

`createdDate`

`date-time`

The date and time when Xcode Cloud created the build.

`destinationCommit`

CiBuildRun.Attributes.DestinationCommit

Detailed information about the commit of a pull request build’s target branch. This value is only available to builds from pull requests.

`executionProgress`

CiExecutionProgress

A string that indicates the progress of the build action.

`finishedDate`

`date-time`

The date and time when Xcode Cloud completed the build.

`isPullRequestBuild`

`boolean`

A Boolean value that indicates whether the build was started by a change to a pull request.

`issueCounts`

CiIssueCounts

An integer value that represents the number of issues Xcode Cloud encountered when it performed the build.

`number`

`integer`

The Xcode Cloud build number.

`sourceCommit`

CiBuildRun.Attributes.SourceCommit

Detailed information about the commit of a pull request build’s source branch. This value is only available to builds from pull requests.

`startedDate`

`date-time`

The date and time when Xcode Cloud started the build.

`startReason`

`string`

A string that indicates what started the build.

Possible Values: `GIT_REF_CHANGE, MANUAL, MANUAL_REBUILD, PULL_REQUEST_OPEN, PULL_REQUEST_UPDATE, SCHEDULE`

## Topics

### Objects and Types

object CiBuildRun.Attributes.DestinationCommit

The latest commit of a pull request’s target branch or the source commit for builds that aren’t pull request builds.

object CiBuildRun.Attributes.SourceCommit

The latest commit of a Git branch or tag, or of a pull request’s source branch.

object CiGitUser

The data structure that represents a Git Users resource.

object CiIssueCounts

The data structure that represents an Issue Counts resource.

type CiCompletionStatus

A string that represents the completion status of an Xcode Cloud build.

type CiExecutionProgress

A string that represents the progress of an ongoing Xcode Cloud build.

## See Also

### Objects

object CiBuildRun.Relationships

The relationships of the Build Runs resource you included in the request and those on which you can operate.

