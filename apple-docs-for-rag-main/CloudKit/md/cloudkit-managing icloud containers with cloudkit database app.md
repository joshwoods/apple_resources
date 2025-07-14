

- CloudKit
-  Managing iCloud Containers with CloudKit Database App 

# Managing iCloud Containers with CloudKit Database App

Inspect and modify the schema and data for your app’s iCloud container.

## Overview

The CloudKit Database app is a web-based tool for developers to manage their iCloud containers. You can sign in to the CloudKit Database app through the Apple Developer web portal or through the CloudKit Console at https://icloud.developer.apple.com/.

With the CloudKit Database app, you can:

- See all the containers for your account.

- View and edit your development schema, and view your production schema.

- View and edit your test data during development or debugging.

- View logs and metrics for your containers.

- Deploy your schema to production. See Deploying an iCloud Container’s Schema.

- Obtain API tokens for use with CloudKit web services and CloudKit JS. See Obtaining an API Token for an iCloud Container.

### Navigate to an iCloud Container’s Schema Management Page

A schema defines record types and the possible relationships between them. You can use CloudKit Database Console or code to create your app’s schema. If you use code to create a just-in-time schema, the CloudKit Database app can help you verify the schema is correct.

To navigate to the iCloud container’s schema management page:

1.  Sign in to CloudKit Console at https://icloud.developer.apple.com/.

2.  Select the CloudKit Database from the app list.

3.  From the container selection drop-down at the top of the page, choose your app’s container.

4.  Click the Record Types menu item in the Schema section to open the container’s schema management page.

After you select the container you want to manage, you can access information about the schema quickly by using the menu items. See Inspecting and Editing an iCloud Container’s Schema for more details.

### Navigate to an iCloud container’s data management page

You can use the CloudKit Database app to inspect data within the public database of an iCloud container. If you develop using the same iCloud account to store private data, you can also use the CloudKit Database app to inspect and edit private data.

Don’t use the CloudKit Database app as a general data editor. Although you can create, modify, and delete records using CloudKit Dashboard, the intent of this functionality is to help you debug your schema during the design phase.

To navigate to the iCloud container’s data management page:

1.  Sign in to CloudKit Console at https://icloud.developer.apple.com/.

2.  Select the CloudKit Database from the app list.

3.  From the container selection drop-down at the top of the page, choose your app’s container.

4.  Click the Records menu item in the Data section to open the container’s data management page.

For more information about inspecting a container’s data, see Handling an iCloud Container’s Data.

## Topics

### Container Management

Inspecting and Editing an iCloud Container’s Schema

Review and edit the schema for your app’s container using the CloudKit Database app.

Handling an iCloud Container’s Data

Inspect and manage your app’s iCloud container data using the CloudKit Database app.

Deploying an iCloud Container’s Schema

Reset your container’s state during development and deploy your container’s schema to production.

Obtaining an API Token for an iCloud Container

Generate an API token to access CloudKit web services or use CloudKit JS.

## See Also

### Schemas

Designing and Creating a CloudKit Database

Create a schema to store your app’s objects as records in iCloud using CloudKit.

class CKRecordZone

A database partition that contains related records.

class CKRecord

A collection of key-value pairs that store your app’s data.

class Reference

A relationship between two records in a record zone.

class CKAsset

An external file that belongs to a record.

Integrating a Text-Based Schema into Your Workflow

Define and update your schema with the CloudKit Schema Language.

