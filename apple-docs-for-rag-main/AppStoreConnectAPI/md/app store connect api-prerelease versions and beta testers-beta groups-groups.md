

- App Store Connect API
- Prerelease Versions and Beta Testers
-  Beta Groups 

API Collection

# Beta Groups

Groups of beta testers that have access to one or more builds.

## Overview

A `betaGroups` resource represents the group of testers that have access to builds for testing. Each beta group is associated with a single app and contains one or more builds. Every tester has access to every build in the group.

There are two types of beta tester groups:

- Internal beta tester — Contains members of your App Store Connect team whom you’ve designated as beta testers. For more information about internal testers, seeAdd internal testers.

- External beta tester — You create and manage these groups. They may contain individuals from your company who don’t qualify as internal testers, or people outside of your organization that you’ve invited to test your app. For more information about external testers, see Invite external testers.

Add beta testers to a group through App Store Connect or with this API.

## Topics

### Creating, Modifying, and Deleting Beta Groups

Create a Beta Group

Create a beta group associated with an app, optionally enabling TestFlight public links.

Modify a Beta Group

Modify a beta group’s metadata, including changing its Testflight public link status.

Delete a Beta Group

Delete a beta group and remove beta tester access to associated builds.

### Getting Beta Group Information

List Beta Groups

Find and list beta groups for all apps.

Read Beta Group Information

Get a specific beta group.

Read the App Information of a Beta Group

Get the app information for a specific beta group.

Read metrics for beta testers in a beta group

Get beta tester usage metrics for a beta group.

Read recruitment criteria for a beta group

Get the recruitment criteria information for a specific beta group.

Read build compatibilty for a beta group

Get the build compatibilty information for a specific beta group.

### Adding and Removing Builds and Testers

Add Beta Testers to a Beta Group

Add a specific beta tester to one or more beta groups for beta testing.

Remove Beta Testers from a Beta Group

Remove a specific beta tester from a one or more beta groups, revoking their access to test builds associated with those groups.

Add Builds to a Beta Group

Associate builds with a beta group to enable the group to test the builds.

Remove Builds from a Beta Group

Remove access to test one or more builds from beta testers in a specific beta group.

### Reading Build and Beta Tester Information

List All Builds for a Beta Group

Get a list of builds associated with a specific beta group.

Get All Build IDs in a Beta Group

Get a list of build resource IDs in a specific beta group.

List All Beta Testers in a Beta Group

Get a list of beta testers contained in a specific beta group.

Get All Beta Tester IDs in a Beta Group

Get a list of the beta tester resource IDs in a specific beta group.

### Measuring public link usage

Read public link usage metrics for a beta group

Get public link usage metrics for a specific beta group.

### Objects

object BetaGroup

The data structure that represents a Beta Groups resource.

object BetaGroupResponse

A response that contains a single Beta Groups resource.

object BetaGroupsWithoutIncludesResponse

A response body that contains a list of beta groups without any includes.

object BetaGroupCreateRequest

The request body you use to create a Beta Group.

object BetaGroupUpdateRequest

The request body you use to update a Beta Group.

object BetaGroupBuildsLinkagesRequest

A request body you use to add or remove builds from a beta group.

object BetaGroupBetaTestersLinkagesRequest

A request body you use to add or remove beta testers from a beta group.

object BetaGroupBetaTestersLinkagesResponse

A response body that contains a list of related resource IDs.

object BetaGroupBuildsLinkagesResponse

A response body that contains a list of related resource IDs.

object BetaPublicLinkUsagesV1MetricResponse

object BetaGroupsResponse

A response that contains a list of Beta Group resources.

## See Also

### Beta Testers and Groups

Beta Testers

People who can install and test prerelease builds.

Beta Tester Invitations

Requests to send or resend an email inviting a beta tester to test an app.

Beta recruitment criteria

Create public links that accept testers with specific device and OS combinations.

