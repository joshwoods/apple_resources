

- Core Data
-  Modeling data 

Article

# Modeling data

Configure the data model file to contain your app’s object graph.

## Overview

A data model holds information about your application’s objects and the graph of how objects relate to each other. You provide this information in your project’s `.xcdatamodeld` file package. To add a data model to your project, see Creating a Core Data model.

This screenshot shows the data model for an app that displays a feed of earthquake data.

Model your data by describing your objects as entities, adding their properties as attributes and relationships, and finally generating respective NSManagedObject subclasses to inherit change tracking and life cycle management.

## Topics

### Configuring a Core Data Model

Configuring Entities

Model your app’s objects.

Configuring Attributes

Describe the properties that compose an entity.

Configuring Relationships

Specify how entities relate and how change propagates between them.

Generating code

Automatically or manually generate managed object subclasses from entities.

## See Also

### Data modeling

Core Data model

Describe your app’s object structure.

