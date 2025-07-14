

- App Store Connect API
-  CiCompletionStatus 

Type

# CiCompletionStatus

A string that represents the completion status of an Xcode Cloud build.

App Store Connect API 1.5+

``` source
string CiCompletionStatus
```

## Possible Values 

`SUCCEEDED`  

`FAILED`  

`ERRORED`  

`CANCELED`  

`SKIPPED`  

## Possible values

SUCCEEDED  
Xcode Cloud successfully completed a build.

FAILED  
The Xcode Cloud build failed; for example, if you configure the Required to Pass setting for a test action and a unit test fails. For more information, see Add a Test Action in Configuring your Xcode Cloud workflow’s actions.

ERRORED  
Xcode Cloud encountered an internal error when it performed the build.

CANCELED  
Xcode Cloud canceled the build because you manually canceled an ongoing build or because you enabled the Auto-cancel Builds setting for a workflow. For more information about the Auto-cancel Builds setting, see Xcode Cloud workflow reference.

SKIPPED  
Xcode Cloud skipped the build; for example, if you configure the Auto- termcancel Builds setting for a workflow and push many changes in quick succession.

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

type CiExecutionProgress

A string that represents the progress of an ongoing Xcode Cloud build.

