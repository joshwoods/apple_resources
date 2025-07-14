

- Contacts
-  Accessing a person’s contact data using Contacts and ContactsUI 

Sample Code

# Accessing a person’s contact data using Contacts and ContactsUI

Allow people to grant your app access to contact data by adding the Contact access button and Contact access picker to your app.

Download

iOS 18.0+iPadOS 18.0+Xcode 16.0+

## Overview

Note

This sample code project is associated with WWDC24 session 10121: Meet the Contact Access Button.

### Configure the sample code project

Before running the sample code project in Xcode, select the sample target, then configure it to use your Developer team for signing.

## See Also

### Essentials

Accessing the contact store

Request permission from the person to read and write their contact data.

class CNContactStore

The object that fetches and saves contacts, groups, and containers from the user’s Contacts database.

NSContactsUsageDescription

A message that tells the user why the app is requesting access to the user’s contacts.

com.apple.developer.contacts.notes

A Boolean value that indicates whether the app may access the notes in contact entries.

