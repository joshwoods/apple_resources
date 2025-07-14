

- Device Management
-  Commands and Queries 

API Collection

# Commands and Queries

Manage the configuration and behavior of your devices.

## Overview

The Mobile Device Management (MDM) protocol provides a way to tell a device to remotely execute certain management commands or queries. First, a device registers with the MDM server. Then, the server sends push notifications to the device when there are commands to process on the device.

When the device receives the notification, it polls the server for the command, processes the command, and reports the command results to the server. The device then checks for other commands to process.

Important

Mobile Device Management is for enterprise use only. To use it in your app, the Account Holder of your app’s development team must request the Mobile Device Management capability. See Request a Mobile Device Management Capability.

## Topics

### Profile Management

Install a Profile

Install a configuration profile on a device.

List the Installed Profiles

Get a list of installed profiles on a device.

Remove a Profile

Remove a previously installed profile from the device.

Install a Provisioning Profile

Install a provisioning profile on a device.

List the Installed Provisioning Profiles

Get a list of installed provisioning profiles on a device.

Remove a Provisioning Profile

Remove a previously installed provisioning profile from a device.

### Device Details

List the Installed Apps

Get a list of the installed apps on a device.

Get Device Information

Get detailed information about a device.

Release Device from Await Configuration

Inform the device that it can allow the user to continue in Setup Assistant.

User Configured Command

Informs the device that it can continue past Setup Assistant and finish login.

List the Installed Restrictions

Get a list of restrictions on the device.

### Device State

Erase a Device

Remotely and immediately erase a device.

Lock a Device

Remotely and immediately lock a device.

Restart a Device

Remotely and immediately restart a device.

Shut Down a Device

Remotely and immediately shut down a device.

### Managed Apps

Install an App

Install a third-party app on a device.

Install an Enterprise App

Install an enterprise app on a device.

Apply a Redemption Code

Complete the installation of an app using a redemption code.

Remove an App

Remove an installed managed app.

Validate Apps

Force validation of developer and universal provisioning profiles for enterprise apps.

List the Managed Apps

Get the status of all managed apps on a device.

Query App Attributes

Query attributes in managed apps on a device.

Get App Configuration

Get app configurations from managed apps on a device.

Get App Feedback

Get app feedback from a managed app on the device.

### Managed Media

Install Media

Install a book on a device.

List the Managed Media

Get a list of the managed books on a device.

Remove Media

Remove a previously installed book from a device.

### Accounts

Account Configuration

Create and configure a local administrator account on a device.

Invite to the Program

Invite a user to join the Volume Purchase Program (VPP).

### Passwords

Clear the Passcode

Remove the passcode from a device.

Clear the Restrictions Password

Clear the restrictions password and the restrictions on a device.

Unlock a User Account

Unlock a user account that the system locked because of too many failed password attempts.

Set the Local Administrator Password

Update the local administrator account password.

Set the Firmware Password

Change or clear the firmware password on a device.

Verify the Firmware Password

Verify the firmware password on a device.

### Updates

Schedule an OS Update Scan

Schedule a background scan for operating-system updates on a device.

List the Available OS Updates

Get a list of available operating-system updates for a device.

Schedule an OS Update

Schedule an update of the operating system on a device.

Get the OS Update Status

Get the status of operating-system updates on a device.

### Lost Device

Enable Lost Mode

Enable Lost Mode on a device, which provides a message and phone number on the Lock screen.

Get the Location of a Device

Request the location of a device when in Lost Mode.

Play the Lost Mode Sound

Play the Lost Mode sound on a device that’s in Lost Mode.

Disable Lost Mode

Take the device out of Lost Mode.

### Recovery Lock

Set Recovery Lock Command

Set or clear the Recovery Lock password.

Verify Recovery Lock Command

Verify the device’s Recovery Lock password.

### Content Caching

Content Caching Information Command

Get the status of the content caches on a device.

### AirPlay Mirroring

Start AirPlay Mirroring

Prompt the user to share their screen using AirPlay Mirroring.

Stop AirPlay Mirroring

Stop mirroring the display on another device.

### eSim Management

Update the eSIM Cellular Plan

Query a carrier URL for active eSIM cellular-plan profiles on a device.

### Managed Settings

Disable Remote Desktop

Disable Remote Desktop on a device.

Enable Remote Desktop

Enable Remote Desktop on a device.

Configure Settings

Configure settings on a device.

### Lights-Out Management

LOM Device Request Command

Send requests to a device using lights-out management (LOM).

LOM Setup Request Command

Get information from a device to set up lights-out management (LOM).

### Security

Security Information

Get security-related information about a device.

List the Certificates

Get a list of installed certificates on a device.

Get the Bypass Code for Activation Lock

Get the code to bypass Activation Lock on a device.

Clear the Bypass Code for Activation Lock

Clear the Activation Lock bypass code on a device.

Rotate the FileVault Key

Change the FileVault primary password on a device.

### Extensions

List Active NSExtensions

Get a list of active extensions for a user on a device.

List the NSExtensions

Get a list of the installed extensions for a user on a device.

### User Management

List the User Accounts

Get a list of users with active accounts on a device.

Log Out the User

Force the current user to log out of a device.

Delete a User

Delete a user’s account from a device.

### Declarative Management

Enable Declarative Management

Enable your server to support declarative management or trigger a declarative management synchronization operation on the device.

### Deprecated

Request the Unlock Token

Request an unlock token from a device.

Deprecated

## See Also

### MDM Protocol

Implementing Device Management

Set up an MDM server and send commands to managed devices.

Check-in

Authenticate devices and maintain push tokens with these commands.

User Enrollment

Authenticate devices using an user identity focused workflow.

