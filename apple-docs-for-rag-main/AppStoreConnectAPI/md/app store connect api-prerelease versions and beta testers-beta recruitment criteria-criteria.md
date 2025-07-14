

- App Store Connect API
- Prerelease Versions and Beta Testers
-  Beta recruitment criteria 

API Collection

# Beta recruitment criteria

Create public links that accept testers with specific device and OS combinations.

## Overview

Use the `betaRecruitmentCriteria` resource to create public links with Device and OS criteria that help improve beta recruitment. Gain insights on the public-link performance from tester-event metrics, so you can modify the criteria set for the public, and enable or disable a public link.

Team keys or individual keys with these roles can use this this resource:

- Account holder

- Admin

- App Managers

## Topics

### Resending Invitations

Create recruitment criteria

Create new criteria for recruiting testers for your TestFlight build.

Modify recruitment criteria

Update the recruitment criteria for your TestFlight build.

Remove recruitment criteria 

Remove the recruitment criteria for your TestFlight build.

Read recruitment criteria for a beta group

Get the recruitment criteria information for a specific beta group.

Read build compatibilty for a beta group

Get the build compatibilty information for a specific beta group.

Read recruitment criteria options

Get a list of the possible beta recruitment criteria options.

### Objects

object BetaRecruitmentCriterionCompatibleBuildCheck

The data structure that represents a beta recruitment criteria-compatible, build-check resource.

object BetaRecruitmentCriterionCompatibleBuildCheckResponse

A response that contains a single beta recruitment criteria-compatible, build-check resource.

object BetaRecruitmentCriterion

The data structure that represents a beta recruitment criterion resource.

object BetaRecruitmentCriterionCreateRequest

The request body you use to create a beta recruitment criterion.

object BetaRecruitmentCriterionOption

object BetaRecruitmentCriterionResponse

A response that contains a single beta recruitment criterion resource.

object BetaRecruitmentCriterionUpdateRequest

The request body you use to update a beta recruitment criterion resource.

object BetaPublicLinkUsagesV1MetricResponse

type DeviceFamily

String that represents a device family.

object DeviceFamilyOsVersionFilter

The object that you use to specify a device family and operating system to use for your beta recruitment criteria.

object BetaRecruitmentCriterionOptionsResponse

## See Also

### Beta Testers and Groups

Beta Testers

People who can install and test prerelease builds.

Beta Tester Invitations

Requests to send or resend an email inviting a beta tester to test an app.

Beta Groups

Groups of beta testers that have access to one or more builds.

