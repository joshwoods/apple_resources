

- Enterprise Program API
-  User Invitations 

API Collection

# User Invitations

Email invitations to join your Enterprise Program team.

## Overview

The `userInvitations` resource represents users who have been invited to join a team in the Apple Developer website. When you create a user invitation the user receives an email with a link to activate an account and connect it to their Apple Account.

If the user accepts the invitation, the user is added to the team and the invitation is deleted. User invitations expire after three days.

You can also get a list of all invited users and read the invite information of a single user.

## Topics

### Getting Invited Users

List Invited Users

Get a list of pending invitations to join your team.

Read user invitation information

Get information about a pending invitation to join your team.

### Sending and Canceling Invitations

Invite a User

Invite a user with assigned user roles to join your team.

Cancel a User Invitation

Cancel a pending invitation for a user to join your team.

### Objects

object UserInvitation

The data structure that represents a User Invitations resource.

object UserInvitationCreateRequest

The request body you use to create a User Invitation.

object UserInvitationResponse

A response that contains a single User Invitations resource.

object UserInvitationsResponse

A response that contains a list of User Invitations resources.

## See Also

### Users and Roles

Users

Manage users on your Enterprise Program team.

