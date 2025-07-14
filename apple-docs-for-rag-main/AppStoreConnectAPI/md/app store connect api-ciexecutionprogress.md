

- App Store Connect API
-  CiExecutionProgress 

Type

# CiExecutionProgress

A string that represents the progress of an ongoing Xcode Cloud build.

App Store Connect API 1.5+

``` source
string CiExecutionProgress
```

## Possible Values 

`PENDING`  

`RUNNING`  

`COMPLETE`  

## Possible Values

PENDING  
Xcode Cloud hasn’t started the build.

RUNNING  
Xcode Cloud is performing the build.

COMPLETE  
Xcode Cloud completed the build.

## See Also

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

