

- Enterprise Program API
-  Users 

API Collection

# Users

Manage users on your Enterprise Program team.

## Overview

The `users` resource represents an Enteprise Program user. You can change or delete users, but you cannot add them directly. To add users, create a `userInvitation`. The Apple Developer website adds the user to your team when they accept the invitation.

## Topics

### Getting User Information

List Users

Get a list of the users on your team.

Read User Information

Get information about a user on your team, such as name, roles, and app visibility.

### Modifying and Removing User Accounts

Modify a User Account

Change a user’s role, app visibility information, or other account details.

Delete a User Account

Remove a user from your team.

### Objects and Data Types

object User

The data structure that represents a Users resource.

object UserUpdateRequest

The request body you use to update a User.

object UserResponse

A response that contains a single Users resource.

object UsersResponse

A response that contains a list of Users resources.

type UserRole

Strings that represent user roles and permissions in the Apple Developer website.

## See Also

### Users and Roles

User Invitations

Email invitations to join your Enterprise Program team.

