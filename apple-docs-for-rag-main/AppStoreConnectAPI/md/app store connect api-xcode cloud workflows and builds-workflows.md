

- App Store Connect API
- Xcode Cloud Workflows and Builds
-  Workflows 

API Collection

# Workflows

Manage Xcode Cloud workflows and view workflow details like actions and start conditions.

## Overview

The `ciWorkflows` resource represents an Xcode Cloud workflow. Use it to:

- Read workflow information.

- Create a new workflow.

- Update an existing workflow.

- Delete a workflow you no longer need.

To learn more about workflows, see Xcode Cloud workflow reference.

Important

Deleting a workflow also deletes associated build information and artifacts. Instead of deleting a workflow, consider deactivating it in Xcode or App Store Connect. To learn more about deactivating a workflow, see Developing a workflow strategy for Xcode Cloud.

This resource supports JSON web tokens with a lifetime of up to six months. For more information, see Determine the Appropriate Token Lifetime.

## Topics

### Getting Xcode Cloud Workflows

Read Xcode Cloud Workflow Information

Get information about a specific Xcode Cloud workflow.

List All Xcode Cloud Builds for a Workflow

List all builds Xcode Cloud performed for a specific workflow.

Read the Repository Information for an Xcode Cloud Workflow

Get information about the Git repository of a specific Xcode Cloud workflow.

### Managing Xcode Cloud Workflows

Create a Workflow

Create a new Xcode Cloud workflow for an Xcode Cloud product.

Update an Xcode Cloud Workflow

Make changes to an Xcode Cloud workflow.

Delete a Workflow

Delete an Xcode Cloud workflow and all of its associated data.

### Objects and Types

object CiWorkflow

The data structure that represents a Workflows resource.

object CiAction

The data structure that represents an Xcode Cloud workflow action resource.

object CiWorkflowCreateRequest

The request body you use to create a new Xcode Cloud workflow.

object CiWorkflowUpdateRequest

The request body you use to update an Xcode Cloud workflow.

object CiWorkflowResponse

A response that contains a single Workflows resource.

object CiWorkflowsResponse

A response that contains a list of Workflows resources.

object CiBuildRunsResponse

A response that contains a list of Build Runs resources.

object CiManualBranchStartCondition

object CiManualPullRequestStartCondition

object CiManualTagStartCondition

## See Also

### Xcode Cloud Products and Workflows

Products

Read information about the products Xcode Cloud detected or delete a product and all its associated information.

macOS Versions

Read macOS version information you configure for an Xcode Cloud workflow.

Xcode Versions

Read Xcode version information you configure for an Xcode Cloud workflow.

