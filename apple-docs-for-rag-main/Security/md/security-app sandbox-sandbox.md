

- Security
-  App Sandbox 

# App Sandbox

Restrict access to system resources and user data in macOS apps to contain damage if an app becomes compromised.

## Overview

App Sandbox provides protection to system resources and user data by limiting your app’s access to resources requested through entitlements.

Important

To distribute a macOS app through the Mac App Store, you must enable the App Sandbox capability.

## Topics

### Essentials

App Sandbox Entitlement

A Boolean value that indicates whether the app may use access control technology to contain damage to the system and user data if an app is compromised.

Protecting user data with App Sandbox

Guard user data and operating system resources from malicious attacks by limiting your app’s access to files, network connections, and hardware capabilities.

Embedding a command-line tool in a sandboxed app

Add a command-line tool to a sandboxed app’s Xcode project so the resulting app can run it as a helper tool.

Discovering and diagnosing App Sandbox violations

Determine when your macOS app behaves incorrectly because of a sandbox violation, and fix sandbox-related issues.

### Network

com.apple.security.network.server

A Boolean value indicating whether your app may listen for incoming network connections.

com.apple.security.network.client

A Boolean value indicating whether your app may open outgoing network connections.

### Hardware

Camera entitlement

A Boolean value that indicates whether the app may interact with the built-in and external cameras, and capture movies and still images.

com.apple.security.device.microphone

A Boolean value that indicates whether the app may use the microphone.

com.apple.security.device.usb

A Boolean value indicating whether your app may interact with USB devices.

com.apple.security.print

A Boolean value indicating whether your app may print a document.

com.apple.security.device.bluetooth

A Boolean value indicating whether your app may interact with Bluetooth devices.

### App Data

Address book entitlement

A Boolean value that indicates whether the app may have read-write access to contacts in the user’s address book.

Location entitlement

A Boolean value that indicates whether the app may access location information from Location Services.

Calendars entitlement

A Boolean value that indicates whether the app may have read-write access to the user’s calendar.

### File Access

Accessing files from the macOS App Sandbox

Read and write documents and supporting files while maintaining security protection.

Migrating your app’s files to its App Sandbox container

Simplify your app’s access to documents and supporting files.

com.apple.security.files.user-selected.read-only

A Boolean value that indicates whether the app may have read-only access to files the user has selected using an Open or Save dialog.

com.apple.security.files.user-selected.read-write

A Boolean value that indicates whether the app may have read-write access to files the user has selected using an Open or Save dialog.

com.apple.security.files.downloads.read-only

A Boolean value that indicates whether the app may have read-only access to the Downloads folder.

com.apple.security.files.downloads.read-write

A Boolean value that indicates whether the app may have read-write access to the Downloads folder.

com.apple.security.assets.pictures.read-only

A Boolean value that indicates whether the app may have read-only access to the Pictures folder.

com.apple.security.assets.pictures.read-write

A Boolean value that indicates whether the app may have read-write access to the Pictures folder.

com.apple.security.assets.music.read-only

A Boolean value that indicates whether the app may have read-only access to the Music folder.

com.apple.security.assets.music.read-write

A Boolean value that indicates whether the app may have read-write access to the Music folder.

com.apple.security.assets.movies.read-only

A Boolean value that indicates whether the app may have read-only access to the Movies folder.

com.apple.security.assets.movies.read-write

A Boolean value that indicates whether the app may have read-write access to the Movies folder.

All files entitlement

A Boolean value that indicates whether the app may have access to all files.

Deprecated

NSAppDataUsageDescription

A message that tells the user why the app needs to access files in other apps’ sandbox containers.

