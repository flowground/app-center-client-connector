# ![LOGO](logo.png) App Center Client **flow**ground Connector

## Description

A generated **flow**ground connector for the App Center Client API (version preview).

Generated from: https://api.appcenter.ms/preview/swagger.json<br/>
Generated at: 2019-07-11T12:18:06+02:00

## API Description

Microsoft Visual Studio App Center API

## Authorization

Supported authorization schemes:
- API Key- Basic Authentication

## Actions

### Registers a user for an existing device

*Tags:* `distribute`

#### Input Parameters
* `user_id` - _required_ - The ID of the user

### Get Default email notification settings for the user

*Tags:* `alerting`

### Rejects a pending organization invitation

*Tags:* `account`

#### Input Parameters
* `invitation_token` - _required_ - The app invitation token that was sent to the user

### Accepts a pending organization invitation for the specified user

*Tags:* `account`

#### Input Parameters
* `invitation_token` - _required_ - The app invitation token that was sent to the user

### Accepts all pending invitations to distribution groups for the specified user

*Tags:* `account`

### Rejects a pending invitation for the specified user

*Tags:* `account`

#### Input Parameters
* `invitation_token` - _required_ - The app invitation token that was sent to the user

### Accepts a pending invitation for the specified user

*Tags:* `account`

#### Input Parameters
* `invitation_token` - _required_ - The app invitation token that was sent to the user

### Gets all service connections of the service type for GDPR export.

*Tags:* `account`

### DataSubjectRight_CancelExportRequest

*Tags:* `gdpr`

#### Input Parameters
* `token` - _required_ - Unique request ID (GUID)

### DataSubjectRight_ExportStatusRequest

*Tags:* `gdpr`

#### Input Parameters
* `token` - _required_ - Unique request ID (GUID)

### DataSubjectRight_ExportRequest

*Tags:* `gdpr`

### DataSubjectRight_CancelDeleteRequest

*Tags:* `gdpr`

#### Input Parameters
* `token` - _required_ - Unique request ID (GUID)

### DataSubjectRight_DeleteStatusRequest

*Tags:* `gdpr`

#### Input Parameters
* `token` - _required_ - Unique request ID (GUID)
* `email` - _required_ - Email used for delete with x-authz-bypass headers

### DataSubjectRight_DeleteRequest

*Tags:* `gdpr`

### Returns the device details.

*Tags:* `distribute`

#### Input Parameters
* `device_udid` - _required_ - The UDID of the device

### Removes an existing device from a user

*Tags:* `distribute`

#### Input Parameters
* `device_udid` - _required_ - The UDID of the device

### Returns all devices associated with the given user.

*Tags:* `distribute`

### Returns the user profile data

*Tags:* `account`

### Updates the user profile and returns the updated user data

*Tags:* `account`

### Return a list of applications that the user has tester permission to with the latest release for each.

*Tags:* `distribute`

### If 'latest' is not specified then it will return the specified release if it's enabled. If 'latest' is specified, regardless of whether a release hash is provided, the latest enabled release is returned.

*Tags:* `distribute`

#### Input Parameters
* `app_secret` - _required_ - The secret of the target application
* `release_hash` - _required_ - The hash of the release or 'latest' to get the latest release from all the distribution groups assigned to the current user.
* `udid` - _optional_ - When passing `udid` in the query string, a provisioning check for the given device ID will be done. Will be ignored for non-iOS platforms.

### Get a release with 'latest' for the given public group.

*Tags:* `distribute`

#### Input Parameters
* `app_secret` - _required_ - The secret of the target application
* `distribution_group_id` - _required_ - the id for destination

### Public webhook sink

*Tags:* `build`

### Check for updates

*Tags:* `codepush`

#### Input Parameters
* `deployment_key` - _required_
* `app_version` - _required_
* `package_hash` - _optional_
* `label` - _optional_
* `client_unique_id` - _optional_
* `is_companion` - _optional_
* `previous_label_or_app_version` - _optional_
* `previous_deployment_key` - _optional_

### Returns the acquisition service status to the caller

*Tags:* `codepush`

### Report download of specified release

*Tags:* `codepush`

### Report Deployment status metric

*Tags:* `codepush`

### Notify download(s) for the provided distribution release(s).

*Tags:* `distribute`

#### Input Parameters
* `owner_name` - _required_ - The name of the app owner
* `app_name` - _required_ - The name of the app

### Returns the manifest.plist in XML format for installing the release on a device. Only available for iOS.

*Tags:* `distribute`

#### Input Parameters
* `app_id` - _required_ - The ID of the application
* `release_id` - _required_ - The release_id
* `token` - _required_ - A hash that authorizes the download if it matches the release info.

### Updates the given organization user

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `user_name` - _required_ - The slug name of the user

### Removes a user from an organization.

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `user_name` - _required_ - The slug name of the user

### Returns a list of users that belong to an organization

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `include_implicit` - _optional_ - Check if the return values should return implicit users.

### Returns a unique list of users including the whole organization members plus testers in any shared group of that org

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name

### Removes a user from a team that is owned by an organization

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `team_name` - _required_ - The team's name
* `user_name` - _required_ - The slug name of the user

### Returns the users of a team which is owned by an organization

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `team_name` - _required_ - The team's name

### Adds a new user to a team that is owned by an organization

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `team_name` - _required_ - The team's name

### Updates the permissions the team has to the app

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `team_name` - _required_ - The team's name
* `app_name` - _required_ - The name of the application

### Removes an app from a team

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `team_name` - _required_ - The team's name
* `app_name` - _required_ - The name of the application

### Adds an app to a team

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `team_name` - _required_ - The team's name

### Returns the apps a team has access to

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `team_name` - _required_ - The team's name

### Returns the details of a single team

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `team_name` - _required_ - The team's name

### Deletes a single team

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `team_name` - _required_ - The team's name

### Updates a single team

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `team_name` - _required_ - The team's name

### Returns the list of all teams in this org

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name

### Creates a team and returns it

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name

### Removes a user's invitation to an organization

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `email` - _required_ - The email address of the user to send the password reset mail to.

### Cancels an existing organization invitation for the user and sends a new one

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `email` - _required_ - The email address of the user to send the password reset mail to.

### Allows the role of an invited user to be changed

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `email` - _required_ - The email address of the user to send the password reset mail to.

### Invites a new or existing user to an organization

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name

### Removes a user's invitation to an organization

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name

### Gets the pending invitations for the organization

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name

### Returns a list of distribution groups with details for an organization

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `apps_limit` - _optional_ - The max number of apps to include in the response

### Resend shared distribution group invite notification to previously invited testers

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `distribution_group_name` - _required_ - The name of the distribution group

### Delete apps from distribution group in an org

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `distribution_group_name` - _required_ - The name of the distribution group

### Returns a list of member in the distribution group specified

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `distribution_group_name` - _required_ - The name of the distribution group

### Accepts an array of user email addresses to get added to the specified group

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `distribution_group_name` - _required_ - The name of the distribution group

### Delete apps from distribution group in an org

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `distribution_group_name` - _required_ - The name of the distribution group

### Get apps from a distribution group in an org

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `distribution_group_name` - _required_ - The name of the distribution group

### Add apps to distribution group in an org

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `distribution_group_name` - _required_ - The name of the distribution group

### Returns a single distribution group in org for a given distribution group name

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `distribution_group_name` - _required_ - The name of the distribution group

### Update one given distribution group name in an org

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `distribution_group_name` - _required_ - The name of the distribution group

### Deletes a single distribution group from an org with a given distribution group name

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `distribution_group_name` - _required_ - The name of the distribution group

### Creates a disribution goup which can be shared across apps under an organization

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name

### Returns a list of distribution groups in the org specified

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name

### Returns a list of azure subscriptions for the organization

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name

### Sets the organization avatar

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name

### Deletes the uploaded organization avatar

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name

### Creates a new app for the organization and returns it to the caller

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name

### Returns a list of apps for the organization

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name

### Allows the role of an aad_group to be changed

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `aad_group_id` - _required_ - The unique ID (UUID) of the aad_group

### Delete already added aad group from the organization

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name
* `aad_group_id` - _required_ - The unique ID (UUID) of the aad_group

### Returns a list of aad groups that belong to an organization

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name

### Adds aad groups to an organization

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name

### Returns the details of a single organization

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name

### Returns a list of organizations the requesting user has access to

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name

### Deletes a single organization

*Tags:* `account`

#### Input Parameters
* `org_name` - _required_ - The organization's name

### Aggregated Billing Information for a given Organization.

*Tags:* `billing`

#### Input Parameters
* `orgName` - _required_ - The name of the Organization
* `service` - _optional_ - Type of service that should be included in the Billing Information
    Possible values: Test, Build.
* `period` - _optional_ - Type of period that should be included in the Billing Information
    Possible values: Previous, Current, Next.
* `showOriginalPlans` - _optional_ - Controls whether the API should show the original plan when Azure Subscription is not enabled

### Creates a new organization and returns it to the caller

*Tags:* `account`

### Returns a list of organizations the requesting user has access to

*Tags:* `account`

### Returns all invitations sent by the caller

*Tags:* `account`

### Returns a list of azure subscriptions for the user

*Tags:* `account`

### Gets the Xcode versions available to this app

*Tags:* `build`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Gets the Xamarin SDK bundles available to this app

*Tags:* `build`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Get web hooks configured for a particular app

*Tags:* `alerting`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Available for UWP apps only.

> Gets a list of application versions. Available for UWP apps only.

*Tags:* `crash`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Removes the user from the app

*Tags:* `account`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application
* `user_email` - _required_ - The user email of the user to delete

### Update user permission for the app

*Tags:* `account`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application
* `user_email` - _required_ - The user email of the user to patch

### Returns the users associated with the app specified with the given app name which belongs to the given owner.

*Tags:* `account`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Gets a device set belonging to the user

*Tags:* `test`

#### Input Parameters
* `id` - _required_ - The UUID of the device set
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Updates a device set belonging to the user

*Tags:* `test`

#### Input Parameters
* `id` - _required_ - The UUID of the device set
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Deletes a device set belonging to the user

*Tags:* `test`

#### Input Parameters
* `id` - _required_ - The UUID of the device set
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Lists device sets belonging to the user

*Tags:* `test`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Creates a device set belonging to the user

*Tags:* `test`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Transfers ownership of an app to a new organization

*Tags:* `account`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Transfers ownership of an app to a different user or organization

*Tags:* `account`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application
* `destination_owner_name` - _required_ - The name of the owner (user or organization) to which the app is being transferred

### Returns available toolsets for application

*Tags:* `build`

#### Input Parameters
* `tools` - _optional_ - Toolset name
    Possible values: xamarin, xcode, node.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Delete the given tester from the all releases

*Tags:* `distribute`

#### Input Parameters
* `tester_id` - _required_ - The id of the tester
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Returns the testers associated with the app specified with the given app name which belongs to the given owner.

*Tags:* `account`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Returns list of all test runs for a given test series

*Tags:* `test`

#### Input Parameters
* `test_series_slug` - _required_ - The slug of the test series
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Deletes a single test series

*Tags:* `test`

#### Input Parameters
* `test_series_slug` - _required_ - The slug of the test series
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Updates name and slug of a test series

*Tags:* `test`

#### Input Parameters
* `test_series_slug` - _required_ - The slug of the test series
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Returns list of all test series for an application

*Tags:* `test`

#### Input Parameters
* `query` - _optional_ - A query string to filter test series
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Creates new test series for an application

*Tags:* `test`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Stop a test run execution

*Tags:* `test`

#### Input Parameters
* `test_run_id` - _required_ - The ID of the test run to be stopped
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Gets state of the test run

*Tags:* `test`

#### Input Parameters
* `test_run_id` - _required_ - The ID of the test run
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Starts test run

*Tags:* `test`

#### Input Parameters
* `test_run_id` - _required_ - The ID of the test run
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Returns a single test report

*Tags:* `test`

#### Input Parameters
* `test_run_id` - _required_ - The ID of the test run
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Adds file with the given hash to a test run

*Tags:* `test`

#### Input Parameters
* `test_run_id` - _required_ - The ID of the test run
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Adds file with the given hash to a test run

*Tags:* `test`

#### Input Parameters
* `test_run_id` - _required_ - The ID of the test run
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Uploads file for a test run

*Tags:* `test`

#### Input Parameters
* `test_run_id` - _required_ - The ID of the test run
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Returns a single test runs

*Tags:* `test`

#### Input Parameters
* `test_run_id` - _required_ - The ID of the test run
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Logically deletes a test run

*Tags:* `test`

#### Input Parameters
* `test_run_id` - _required_ - The ID of the test run
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Returns a list of test runs

*Tags:* `test`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Creates a new test run

*Tags:* `test`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Lists test run data

*Tags:* `test`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Lists pipeline test data

*Tags:* `test`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Lists hash file data

*Tags:* `test`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Lists file set file data

*Tags:* `test`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Lists all the endpoints available for Test app data

*Tags:* `test`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Returns the details of all teams that have access to the app.

*Tags:* `account`

#### Input Parameters
* `app_name` - _required_ - The name of the application
* `owner_name` - _required_ - The name of the owner

### Returns a particular symbol by id (uuid) for the provided application

*Tags:* `crash`

#### Input Parameters
* `symbol_id` - _required_ - The ID of the symbol (uuid of the symbol)
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Gets the URL to download the symbol

*Tags:* `crash`

#### Input Parameters
* `symbol_id` - _required_ - The ID of the symbol (uuid of the symbol)
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Marks a symbol by id (uuid) as ignored

*Tags:* `crash`

#### Input Parameters
* `symbol_id` - _required_ - The ID of the symbol (uuid of the symbol)
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Returns a particular symbol by id (uuid) for the provided application

*Tags:* `crash`

#### Input Parameters
* `symbol_id` - _required_ - The ID of the symbol (uuid of the symbol)
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Returns the list of all symbols for the provided application

*Tags:* `crash`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Gets the URL to download the symbol upload

*Tags:* `crash`

#### Input Parameters
* `symbol_upload_id` - _required_ - The ID of the symbol upload
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Gets a symbol upload by id for the specified application

*Tags:* `crash`

#### Input Parameters
* `symbol_upload_id` - _required_ - The ID of the symbol upload
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Commits or aborts the symbol upload process for a new set of symbols for the specified application

*Tags:* `crash`

#### Input Parameters
* `symbol_upload_id` - _required_ - The ID of the symbol upload
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Deletes a symbol upload by id for the specified application

*Tags:* `crash`

#### Input Parameters
* `symbol_upload_id` - _required_ - The ID of the symbol upload
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Gets a list of all uploads for the specified application

*Tags:* `crash`

#### Input Parameters
* `top` - _optional_ - The maximum number of results to return.
* `status` - _optional_ - Filter results by the current status of a symbol upload: * all: all states in the symbol upload process. Includes created, aborted, committed, processing, indexed and failed states * uploaded: all states after package is uploaded. Includes committed, processing, indexed and failed states * processed: symbol upload processing is completed. Includes indexed and failed states.

    Possible values: all, uploaded, processed.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Begins the symbol upload process for a new set of symbols for the specified application

*Tags:* `crash`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Get information about the currently active subscriptions, if any

*Tags:* `test`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Accept a free trial subscription

*Tags:* `test`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Application specific store service status

*Tags:* `distribute`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Gets the repositories available from the source code host

*Tags:* `build`

#### Input Parameters
* `source_host` - _required_ - The source host
    Possible values: github, bitbucket, vsts, gitlab.
* `vstsAccountName` - _optional_ - Filter repositories only for specified account and project, "vstsProjectId" is required
* `vstsProjectId` - _optional_ - Filter repositories only for specified account and project, "vstsAccountName" is required
* `form` - _optional_ - The selected form of the object
    Possible values: lite, full.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Returns the repository build configuration status of the app

*Tags:* `build`

#### Input Parameters
* `includeInactive` - _optional_ - Include inactive configurations if none are active
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Configures the repository for build

*Tags:* `build`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Removes the configuration for the respository

*Tags:* `build`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Returns the resign status to the caller

*Tags:* `distribute`

#### Input Parameters
* `release_id` - _required_ - The ID of the release.
* `resign_id` - _required_ - The ID of the resign operation.
* `include_provisioning_profile` - _optional_ - A boolean value that indicates if the provisioning profile should be return in addition to the status. When set to true, the provisioning profile will be returned only when status is 'complete' or 'preparing_for_testers'.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Update details about the specified tester associated with the release

*Tags:* `distribute`

#### Input Parameters
* `release_id` - _required_ - The ID of the release
* `tester_id` - _required_ - The id of the tester
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Delete the given tester from the release

*Tags:* `distribute`

#### Input Parameters
* `release_id` - _required_ - The ID of the release
* `tester_id` - _required_ - The id of the tester
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Distributes a release to a user

*Tags:* `distribute`

#### Input Parameters
* `release_id` - _required_ - The ID of the release
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Delete the given distribution store from the release

*Tags:* `distribute`

#### Input Parameters
* `release_id` - _required_ - The ID of the release
* `store_id` - _required_ - The id of the distribution store
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Distributes a release to a store

*Tags:* `distribute`

#### Input Parameters
* `release_id` - _required_ - The ID of the release
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Return information about the provisioning profile. Only available for iOS.

*Tags:* `distribute`

#### Input Parameters
* `release_id` - _required_ - The release_id
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Update details about the specified distribution group associated with the release

*Tags:* `distribute`

#### Input Parameters
* `release_id` - _required_ - The ID of the release
* `group_id` - _required_ - The id of the releases destination
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Delete the given distribution group from the release

*Tags:* `distribute`

#### Input Parameters
* `release_id` - _required_ - The ID of the release
* `group_id` - _required_ - The id of the distribution group
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Distributes a release to a group

*Tags:* `distribute`

#### Input Parameters
* `release_id` - _required_ - The ID of the release
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Get a release with id `release_id`. If `release_id` is `latest`, return the latest release that was distributed to the current user (from all the distribution groups).

*Tags:* `distribute`

#### Input Parameters
* `release_id` - _required_ - The ID of the release, or `latest` to get the latest release from all the distribution groups assigned to the current user.
* `udid` - _optional_ - when supplied, this call will also check if the given UDID is provisioned. Will be ignored for non-iOS platforms. The value will be returned in the property is_udid_provisioned.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Update details of a release.

*Tags:* `distribute`

#### Input Parameters
* `release_id` - _required_ - The ID of the release
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Updates a release.

*Tags:* `distribute`

#### Input Parameters
* `release_id` - _required_ - The ID of the release
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Deletes a release.

*Tags:* `distribute`

#### Input Parameters
* `release_id` - _required_ - The ID of the release
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Return detailed information about releases avaiable to a tester.

*Tags:* `distribute`

#### Input Parameters
* `published_only` - _optional_ - when *true*, filters out releases that were uploaded but were never distributed. Releases that under deleted distribution groups will not be filtered out.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Return basic information about releases.

*Tags:* `distribute`

#### Input Parameters
* `published_only` - _optional_ - When *true*, filters out releases that were uploaded but were never distributed. Releases that under deleted distribution groups will not be filtered out.
* `scope` - _optional_ - When the scope is 'tester', only includes releases that have been distributed to groups that the user belongs to.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Commits or aborts the upload process for a release for the specified application

*Tags:* `distribute`

#### Input Parameters
* `upload_id` - _required_ - The ID of the upload
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Begins the upload process for a new release for the specified application.

*Tags:* `distribute`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Get the latest release from every distribution group associated with an application.

*Tags:* `distribute`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Returns whether a push configuration exists for the selected app.

*Tags:* `push`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Get the push configuration for the selected app.

*Tags:* `push`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Set the push configuration for the selected app.

*Tags:* `push`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Delete the push configuration for the selected app.

*Tags:* `push`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Get details about a specific notification.

*Tags:* `push`

#### Input Parameters
* `notification_id` - _required_ - The id of the notification.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Get a list of notifications from the service.

*Tags:* `push`

#### Input Parameters
* `$top` - _optional_ - The maximum number of results to return. (0 will fetch all results)
* `$skiptoken` - _optional_ - The value identifies a starting point in the collection of entities. This parameter along with limit is used to perform pagination.
* `$orderby` - _optional_ - controls the sorting order and sorting based on which column
* `$inlinecount` - _optional_ - Controls whether or not to include a count of all the items across all pages.
    Possible values: allpages, none.
* `include_archived` - _optional_ - Include arhived push notifications
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Send a notification to one or more devices.

*Tags:* `push`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Delete a notification.

*Tags:* `push`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Delete a device with the selected installId.

*Tags:* `push`

#### Input Parameters
* `install_id` - _required_ - device install id
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Get the status of an export operation.

*Tags:* `push`

#### Input Parameters
* `export_id` - _required_ - The id of the export.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Exports information for all devices using Push to Azure Blob Storage

*Tags:* `push`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Gets a device set belonging to the owner

*Tags:* `test`

#### Input Parameters
* `id` - _required_ - The UUID of the device set
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Updates a device set belonging to the owner

*Tags:* `test`

#### Input Parameters
* `id` - _required_ - The UUID of the device set
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Deletes a device set belonging to the owner

*Tags:* `test`

#### Input Parameters
* `id` - _required_ - The UUID of the device set
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Lists device sets belonging to the owner

*Tags:* `test`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Creates a device set belonging to the owner

*Tags:* `test`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Get Email notification settings of user for a particular app

*Tags:* `alerting`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Invites a new or existing user to an app

*Tags:* `account`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application
* `user_email` - _required_ - The email of the user to invite

### Update pending invitation permission

*Tags:* `account`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application
* `user_email` - _required_ - The email of the user to invite

### Removes a user's invitation to an app

*Tags:* `account`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application
* `user_email` - _required_ - The email of the user to invite

### Invites a new or existing user to an app

*Tags:* `account`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Gets the pending invitations for the app

*Tags:* `account`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Gets the state of HockeyApp Crash forwarding for SxS apps

*Tags:* `crash`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Enable HockeyApp crash forwarding for SxS apps

*Tags:* `crash`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Create a new asset to upload a file

*Tags:* `build`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Enable export configuration.

*Tags:* `export`

#### Input Parameters
* `export_configuration_id` - _required_ - The id of the export configuration.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Disable export configuration.

*Tags:* `export`

#### Input Parameters
* `export_configuration_id` - _required_ - The id of the export configuration.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Get export configuration.

*Tags:* `export`

#### Input Parameters
* `export_configuration_id` - _required_ - The id of the export configuration.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Partially update export configuration.

*Tags:* `export`

#### Input Parameters
* `export_configuration_id` - _required_ - The id of the export configuration.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Delete export configuration.

*Tags:* `export`

#### Input Parameters
* `export_configuration_id` - _required_ - The id of the export configuration.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### List export configurations.

*Tags:* `export`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Create new export configuration

*Tags:* `export`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Get session logs by error ID

*Tags:* `errors`

#### Input Parameters
* `errorId` - _required_ - The id of the error
* `date` - _optional_ - Date of data requested
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Error attachment text.

*Tags:* `errors`

#### Input Parameters
* `errorId` - _required_ - The id of the error
* `attachmentId` - _required_ - Error attachment id.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Error attachment location.

*Tags:* `errors`

#### Input Parameters
* `errorId` - _required_ - The id of the error
* `attachmentId` - _required_ - Error attachment id.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### List error attachments.

*Tags:* `errors`

#### Input Parameters
* `errorId` - _required_ - The id of the error
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Errors list based on search parameters

*Tags:* `errors`

#### Input Parameters
* `filter` - _optional_ - A filter as specified in OData notation
* `q` - _optional_ - A query string
* `order` - _optional_ - It controls the order of sorting
    Possible values: desc, asc.
* `sort` - _optional_ - It controls the sort based on specified field
    Possible values: timestamp, errorGroupId, exceptionClassName, exceptionFile, exceptionLine, exceptionMessage, exceptionMethod, deviceName, osVersion, userId.
* `$top` - _optional_ - The maximum number of results to return
* `$skip` - _optional_ - The offset (starting at 0) of the first result to return. This parameter along with limit is used to perform pagination.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Creates and updates the retention settings in days

*Tags:* `errors`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### gets the retention settings in days

*Tags:* `errors`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Percentage of error-free devices by day in the time range based on the selected versions. If SingleErrorTypeParameter is not provided, defaults to handlederror. API will return -1 if crash devices is greater than active devices

*Tags:* `errors`

#### Input Parameters
* `start` - _required_ - Start date time in data in ISO 8601 date time format
* `end` - _optional_ - Last date time in data in ISO 8601 date time format
* `versions` - _optional_
* `appbuild` - _optional_ - app build
* `errorType` - _optional_ - Type of error (handled vs unhandled), excluding All
    Possible values: unhandledError, handledError.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Gets the stack trace for the error group.

*Tags:* `errors`

#### Input Parameters
* `errorGroupId` - _required_ - The id of the error group
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Top OSes of the selected error group.

*Tags:* `errors`

#### Input Parameters
* `errorGroupId` - _required_ - The id of the error group
* `$top` - _optional_ - The maximum number of results to return. (0 will fetch all results till the max number.)
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Top models of the selected error group.

*Tags:* `errors`

#### Input Parameters
* `errorGroupId` - _required_ - The id of the error group
* `$top` - _optional_ - The maximum number of results to return. (0 will fetch all results till the max number.)
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Error Stacktrace details.

*Tags:* `errors`

#### Input Parameters
* `errorGroupId` - _required_ - The id of the error group
* `errorId` - _required_ - The id of the error
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Error location.

*Tags:* `errors`

#### Input Parameters
* `errorGroupId` - _required_ - The id of the error group
* `errorId` - _required_ - The id of the error
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Download details for a specific error.

*Tags:* `errors`

#### Input Parameters
* `errorGroupId` - _required_ - The id of the error group
* `errorId` - _required_ - The id of the error
* `format` - _optional_ - the format of the crash log
    Possible values: json, txt.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Error details.

*Tags:* `errors`

#### Input Parameters
* `errorGroupId` - _required_ - The id of the error group
* `errorId` - _required_ - The id of the error
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Delete a specific error and related attachments and blobs for an app. Searchable data will not be deleted immediately and may take up to 30 days.

*Tags:* `errors`

#### Input Parameters
* `errorGroupId` - _required_ - The id of the error group
* `errorId` - _required_ - The id of the error
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Latest error details.

*Tags:* `errors`

#### Input Parameters
* `errorGroupId` - _required_ - The id of the error group
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Get all errors for group

*Tags:* `errors`

#### Input Parameters
* `errorGroupId` - _required_ - The id of the error group
* `start` - _required_ - Start date time in data in ISO 8601 date time format
* `end` - _optional_ - Last date time in data in ISO 8601 date time format
* `model` - _optional_
* `os` - _optional_
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Percentage of error-free devices by day in the time range. Api will return -1 if crash devices is greater than active devices

*Tags:* `errors`

#### Input Parameters
* `errorGroupId` - _required_ - The id of the error group
* `start` - _required_ - Start date time in data in ISO 8601 date time format
* `end` - _optional_ - Last date time in data in ISO 8601 date time format
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Count of errors by day in the time range of the selected error group with selected version

*Tags:* `errors`

#### Input Parameters
* `errorGroupId` - _required_ - The id of the error group
* `version` - _optional_
* `start` - _required_ - Start date time in data in ISO 8601 date time format
* `end` - _optional_ - Last date time in data in ISO 8601 date time format
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Error group details

*Tags:* `errors`

#### Input Parameters
* `errorGroupId` - _required_ - The id of the error group
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Update error group state

*Tags:* `errors`

#### Input Parameters
* `errorGroupId` - _required_ - The id of the error group
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Error groups list based on search parameters

*Tags:* `errors`

#### Input Parameters
* `filter` - _optional_ - A filter as specified in OData notation
* `q` - _optional_ - A query string
* `order` - _optional_ - It controls the order of sorting
    Possible values: desc, asc.
* `sort` - _optional_ - It controls the sort based on specified field
    Possible values: matchingReportsCount, exceptionClassName, exceptionMessage, exceptionMethod, lastOccurrence.
* `$top` - _optional_ - The maximum number of results to return
* `$skip` - _optional_ - The offset (starting at 0) of the first result to return. This parameter along with limit is used to perform pagination.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### List of error groups

*Tags:* `errors`

#### Input Parameters
* `version` - _optional_
* `appbuild` - _optional_ - app build
* `groupState` - _optional_
* `start` - _required_ - Start date time in data in ISO 8601 date time format
* `end` - _optional_ - Last date time in data in ISO 8601 date time format
* `$orderby` - _optional_ - controls the sorting order and sorting based on which column
* `$top` - _optional_ - The maximum number of results to return. (0 will fetch all results till the max number.)
* `errorType` - _optional_ - Type of error (handled vs unhandled), including All
    Possible values: all, unhandledError, handledError.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Count of crashes or errors by day in the time range based the selected versions. If SingleErrorTypeParameter is not provided, defaults to handlederror.

*Tags:* `errors`

#### Input Parameters
* `version` - _optional_
* `start` - _required_ - Start date time in data in ISO 8601 date time format
* `end` - _optional_ - Last date time in data in ISO 8601 date time format
* `appbuild` - _optional_ - app build
* `errorType` - _optional_ - Type of error (handled vs unhandled), excluding All
    Possible values: unhandledError, handledError.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Get all available versions in the time range.

*Tags:* `errors`

#### Input Parameters
* `start` - _required_ - Start date time in data in ISO 8601 date time format
* `end` - _optional_ - Last date time in data in ISO 8601 date time format
* `$top` - _optional_ - The maximum number of results to return. (0 will fetch all results till the max number.)
* `$skip` - _optional_ - The offset (starting at 0) of the first result to return. This parameter along with limit is used to perform pagination.
* `$filter` - _optional_ - A filter as specified in https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#97-filtering.
* `$inlinecount` - _optional_ - Controls whether or not to include a count of all the items across all pages.
    Possible values: allpages, none.
* `errorType` - _optional_ - Type of error (handled vs unhandled), including All
    Possible values: all, unhandledError, handledError.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Return the Real time Status publishing of release from store.

*Tags:* `distribute`

#### Input Parameters
* `store_name` - _required_ - The name of the store
* `release_id` - _required_ - The id of the release
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Returns publish logs for a particular release published to a particular store

*Tags:* `distribute`

#### Input Parameters
* `store_name` - _required_ - The name of the store
* `release_id` - _required_ - The ID of the realease
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Return the Error Details of release which failed in publishing.

*Tags:* `distribute`

#### Input Parameters
* `store_name` - _required_ - The name of the store
* `release_id` - _required_ - The id of the release
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Return releases published in a store for releaseId and storeId

*Tags:* `distribute`

#### Input Parameters
* `store_name` - _required_ - The name of the store
* `release_id` - _required_ - The name of the store
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### delete the release with release Id

*Tags:* `distribute`

#### Input Parameters
* `store_name` - _required_ - The name of the store
* `release_id` - _required_ - The id of the release
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Return all releases published  in a store

*Tags:* `distribute`

#### Input Parameters
* `store_name` - _required_ - The name of the store
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Returns the latest release published in a store.

*Tags:* `distribute`

#### Input Parameters
* `store_name` - _required_ - The name of the store
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Return the store details for specified store name.

*Tags:* `distribute`

#### Input Parameters
* `store_name` - _required_ - The name of the store
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Update the store.

*Tags:* `distribute`

#### Input Parameters
* `store_name` - _required_ - The name of the store
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### delete the store based on specific store name.

*Tags:* `distribute`

#### Input Parameters
* `store_name` - _required_ - The name of the store
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Create a new external store for the specified application.

*Tags:* `distribute`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Get all the store details from Storage store table for a particular application.

*Tags:* `distribute`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Resend distribution group app invite notification to previously invited testers

*Tags:* `account`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application
* `distribution_group_name` - _required_ - The name of the distribution group

### Return detailed information about a distributed release in a given distribution group.

*Tags:* `distribute`

#### Input Parameters
* `owner_name` - _required_ - The name of the app owner
* `app_name` - _required_ - The name of the app
* `distribution_group_name` - _required_ - The name of the distribution group.
* `release_id` - _required_ - Only supports the constant `latest`, specific IDs are not supported. `latest` will return the latest release in the distribution group.

### Deletes a release with id 'release_id' in a given distribution group.

*Tags:* `distribute`

#### Input Parameters
* `owner_name` - _required_ - The name of the app owner
* `app_name` - _required_ - The name of the app
* `distribution_group_name` - _required_ - The name of the distribution group.
* `release_id` - _required_ - The ID identifying the unique release.

### Return basic information about distributed releases in a given distribution group.

*Tags:* `distribute`

#### Input Parameters
* `distribution_group_name` - _required_ - The name of the distribution group.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Remove the users from the distribution group

*Tags:* `account`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application
* `distribution_group_name` - _required_ - The name of the distribution group

### Returns a list of member details in the distribution group specified

*Tags:* `account`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application
* `distribution_group_name` - _required_ - The name of the distribution group
* `exclude_pending_invitations` - _optional_ - Whether to exclude pending invitations in the response

### Adds the members to the specified distribution group

*Tags:* `account`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application
* `distribution_group_name` - _required_ - The name of the distribution group

### Returns all devices associated with the given distribution group.

*Tags:* `distribute`

#### Input Parameters
* `distribution_group_name` - _required_ - The name of the distribution group.
* `unprovisioned_only` - _optional_ - when true, filters out provisioned devices
* `udids` - _optional_ - multiple UDIDs which should be part of the resulting CSV.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Returns all devices associated with the given distribution group

*Tags:* `distribute`

#### Input Parameters
* `distribution_group_name` - _required_ - The name of the distribution group.
* `release_id` - _optional_ - when provided, gets the provisioning state of the devices owned by users of this distribution group when compared to the provided release.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Returns a single distribution group for a given distribution group name

*Tags:* `account`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application
* `distribution_group_name` - _required_ - The name of the distribution group

### Updates the attributes of distribution group

*Tags:* `account`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application
* `distribution_group_name` - _required_ - The name of the distribution group

### Deletes a distribution group

*Tags:* `account`

#### Input Parameters
* `app_name` - _required_ - The name of the application
* `owner_name` - _required_ - The name of the owner
* `distribution_group_name` - _required_ - The name of the distribution group

### Returns a list of distribution groups in the app specified

*Tags:* `account`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Creates a new distribution group and returns it to the caller

*Tags:* `account`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Gets application level statistics for all missing symbol groups

*Tags:* `crash`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Gets missing symbol crash group by its id

*Tags:* `crash`

#### Input Parameters
* `symbol_group_id` - _required_ - missing symbol crash group id
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Gets top N (ordered by crash count) of crash groups by missing symbol

*Tags:* `crash`

#### Input Parameters
* `top` - _required_ - top N elements
* `filter` - _optional_ - query filter
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### **Warning, this operation is not reversible.**<br/>
> <br/>
>  A successful call to this API will permanently stop ingesting any logs received via SDK for the given installation ID, and cannot be restored. We advise caution when using this API, it is designed to permanently disable collection from a specific installation of the app on a device, usually following the request from a user.

*Tags:* `analytics`

#### Input Parameters
* `install_id` - _required_ - The id of the device
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### **Warning, this operation is not reversible.** <br/>
> <br/>
> A successful call to this API will permanently stop ingesting any logs received via SDK by app_id, and cannot be restored. We advise caution when using this API, it is designed to permanently disable an app_id.

*Tags:* `analytics`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Creates a short ID for a list of devices

*Tags:* `test`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Returns a list of available devices

*Tags:* `test`

#### Input Parameters
* `app_upload_id` - _optional_ - The ID of the test run
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Rollback the latest or a specific release for an app deployment

*Tags:* `codepush`

#### Input Parameters
* `deployment_name` - _required_ - deployment name
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Modifies a CodePush release metadata under the given Deployment

*Tags:* `codepush`

#### Input Parameters
* `deployment_name` - _required_ - deployment name
* `release_label` - _required_ - release label
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Clears a Deployment of releases

*Tags:* `codepush`

#### Input Parameters
* `deployment_name` - _required_ - deployment name
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Gets the history of releases on a Deployment

*Tags:* `codepush`

#### Input Parameters
* `deployment_name` - _required_ - deployment name
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Create a new CodePush release for the specified deployment

*Tags:* `codepush`

#### Input Parameters
* `deployment_name` - _required_ - deployment name
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Promote one release (default latest one) from one deployment to another

*Tags:* `codepush`

#### Input Parameters
* `deployment_name` - _required_ - deployment name
* `promote_deployment_name` - _required_ - deployment name
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Gets all releases metrics for specified Deployment

*Tags:* `codepush`

#### Input Parameters
* `deployment_name` - _required_ - deployment name
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Deletes a CodePush Deployment for the given app

*Tags:* `codepush`

#### Input Parameters
* `deployment_name` - _required_ - deployment name
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Gets a CodePush Deployment for the given app

*Tags:* `codepush`

#### Input Parameters
* `deployment_name` - _required_ - deployment name
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Modifies a CodePush Deployment for the given app

*Tags:* `codepush`

#### Input Parameters
* `deployment_name` - _required_ - deployment name
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Gets a list of CodePush deployments for the given app

*Tags:* `codepush`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Creates a CodePush Deployment for the given app

*Tags:* `codepush`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### data_getResourceProvisioning

*Tags:* `mbaas`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Creates Cosmos DB or attaches an existing one

*Tags:* `mbaas`

#### Input Parameters
* `AC-Authorization-ARM` - _required_
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Gets general data about the provisioned database

*Tags:* `mbaas`

#### Input Parameters
* `AC-Authorization-ARM` - _required_ - ARM token
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Checks that the Azure Cosmos DB account name already exists. A valid account name may contain only lowercase letters, numbers, and the '-' character, and must be between 3 and 31 characters.

*Tags:* `mbaas`

#### Input Parameters
* `accountName` - _required_
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Available for UWP apps only.

> Gets whether the application has any crashes. Available for UWP apps only.

*Tags:* `crash`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Get session logs by crash ID

*Tags:* `analytics`

#### Input Parameters
* `crash_id` - _required_ - The id of the a crash
* `date` - _optional_ - Date of data requested
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Available for UWP apps only.

> Gets content of the text attachment. Available for UWP apps only.

*Tags:* `crash`

#### Input Parameters
* `crash_id` - _required_ - id of a specific crash
* `attachment_id` - _required_ - attachment id
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Available for UWP apps only.

> Gets the URI location to download crash attachment. Available for UWP apps only.

*Tags:* `crash`

#### Input Parameters
* `crash_id` - _required_ - id of a specific crash
* `attachment_id` - _required_ - attachment id
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Available for UWP apps only.

> Gets all attachments for a specific crash. Available for UWP apps only.

*Tags:* `crash`

#### Input Parameters
* `crash_id` - _required_ - id of a specific crash
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Available for UWP apps only.

> Gets a stacktrace for a specific crash. Available for UWP apps only.

*Tags:* `crash`

#### Input Parameters
* `crash_group_id` - _required_ - id of a specific group
* `grouping_only` - _optional_ - true if the stacktrace should be only the relevant thread / exception. Default is false
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Available for UWP apps only.

> Gets a stacktrace for a specific crash. Available for UWP apps only.

*Tags:* `crash`

#### Input Parameters
* `crash_group_id` - _required_ - id of a specific group
* `crash_id` - _required_ - id of a specific crash
* `grouping_only` - _optional_ - true if the stacktrace should be only the relevant thread / exception. Default is false
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Available for UWP apps only.

> Gets the URI location to download json of a specific crash. Available for UWP apps only.

*Tags:* `crash`

#### Input Parameters
* `crash_group_id` - _required_ - id of a specific group
* `crash_id` - _required_ - id of a specific crash
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Available for UWP apps only.

> Gets the native log of a specific crash as a text attachment. Available for UWP apps only.

*Tags:* `crash`

#### Input Parameters
* `crash_group_id` - _required_ - id of a specific group
* `crash_id` - _required_ - id of a specific crash
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Available for UWP apps only.

> Gets the native log of a specific crash. Available for UWP apps only.

*Tags:* `crash`

#### Input Parameters
* `crash_group_id` - _required_ - id of a specific group
* `crash_id` - _required_ - id of a specific crash
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Available for UWP apps only.

> Gets a specific crash for an app. Available for UWP apps only.

*Tags:* `crash`

#### Input Parameters
* `crash_group_id` - _required_ - id of a specific group
* `crash_id` - _required_ - id of a specific crash
* `include_report` - _optional_ - true if the crash should include the raw crash report. Default is false
* `include_log` - _optional_ - true if the crash should include the custom log report. Default is false
* `include_details` - _optional_ - true if the crash should include in depth crash details
* `include_stacktrace` - _optional_ - true if the crash should include the stacktrace information
* `grouping_only` - _optional_ - true if the stacktrace should be only the relevant thread / exception. Default is false
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Available for UWP apps only.

> Delete a specific crash and related attachments and blobs for an app. Available for UWP apps only.

*Tags:* `crash`

#### Input Parameters
* `crash_group_id` - _required_ - id of a specific group
* `crash_id` - _required_ - id of a specific crash
* `retention_delete` - _optional_ - true in that case if the method should skip update counts
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Available for UWP apps only.

> Gets all crashes of a group. Available for UWP apps only.

*Tags:* `crash`

#### Input Parameters
* `crash_group_id` - _required_ - id of a specific group
* `include_report` - _optional_ - true if the crash should include the raw crash report. Default is false
* `include_log` - _optional_ - true if the crash should include the custom log report. Default is false
* `date_from` - _optional_
* `date_to` - _optional_
* `app_version` - _optional_ - version
* `error_type` - _optional_
    Possible values: CrashingErrors, HandledErrors.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Available for UWP apps only.

> Gets a specific group. Available for UWP apps only.

*Tags:* `crash`

#### Input Parameters
* `crash_group_id` - _required_ - id of a specific group
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Available for UWP apps only.

> Updates a group. Available for UWP apps only.

*Tags:* `crash`

#### Input Parameters
* `crash_group_id` - _required_ - id of a specific group
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Available for UWP apps only.

> Gets a list of crash groups and whether the list contains all available groups. Available for UWP apps only.

*Tags:* `crash`

#### Input Parameters
* `last_occurrence_from` - _optional_ - Earliest date when the last time a crash occured in a crash group
* `last_occurrence_to` - _optional_ - Latest date when the last time a crash occured in a crash group
* `app_version` - _optional_ - version
* `group_type` - _optional_
    Possible values: GroupType1, GroupType2.
* `group_status` - _optional_
    Possible values: open, closed, ignored.
* `group_text_search` - _optional_ - A freetext search that matches in crash, crash types, crash stack_traces and crash user
* `$orderby` - _optional_ - the OData-like $orderby argument
    Possible values: last_occurrence asc, last_occurrence desc, count asc, count desc, display_id asc, display_id desc, impacted_users asc, impacted_users desc.
* `continuation_token` - _optional_ - Cassandra request continuation token. The token is used for pagination.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Returns commit information for a batch of shas

*Tags:* `build`

#### Input Parameters
* `hashes` - _required_ - A collection of commit SHAs comma-delimited
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Get the build log

*Tags:* `build`

#### Input Parameters
* `build_id` - _required_ - The build ID
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Gets the download URI

*Tags:* `build`

#### Input Parameters
* `build_id` - _required_ - The build ID
* `download_type` - _required_ - The download type
    Possible values: build, symbols, logs, mapping, bundle.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Distribute a build

*Tags:* `build`

#### Input Parameters
* `build_id` - _required_ - The build ID
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Returns the build detail for the given build ID

*Tags:* `build`

#### Input Parameters
* `build_id` - _required_ - The build ID
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Cancels a build

*Tags:* `build`

#### Input Parameters
* `build_id` - _required_ - The build ID
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Application specific build service status

*Tags:* `build`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Get project issue related to a crash group

*Tags:* `alerting`

#### Input Parameters
* `crash_group_id` - _required_ - CrashGroup Id
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Get bug tracker settings for a particular app

*Tags:* `alerting`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Returns the projects in the repository for the branch, for all toolsets

*Tags:* `build`

#### Input Parameters
* `branch` - _required_ - The branch name
* `os` - _required_ - The desired OS for the project scan; normally the same as the app OS
    Possible values: iOS, Android, Windows, macOS.
* `platform` - _required_ - The desired platform for the project scan
    Possible values: Objective-C-Swift, React-Native, Xamarin, Java, UWP.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Gets the branch configuration

*Tags:* `build`

#### Input Parameters
* `branch` - _required_ - The branch name
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Configures the branch for build

*Tags:* `build`

#### Input Parameters
* `branch` - _required_ - The branch name
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Reconfigures the branch for build

*Tags:* `build`

#### Input Parameters
* `branch` - _required_ - The branch name
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Deletes the branch build configuration

*Tags:* `build`

#### Input Parameters
* `branch` - _required_ - The branch name
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Returns the list of builds for the branch

*Tags:* `build`

#### Input Parameters
* `branch` - _required_ - The branch name
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Create a build

*Tags:* `build`

#### Input Parameters
* `branch` - _required_ - The branch name
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Returns the list of Git branches for this application

*Tags:* `build`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Aggregated Billing Information for owner of a given app.

*Tags:* `billing`

#### Input Parameters
* `service` - _optional_ - Type of service that should be included in the Billing Information
    Possible values: Test, Build.
* `period` - _optional_ - Type of period that should be included in the Billing Information
    Possible values: Previous, Current, Next.
* `showOriginalPlans` - _optional_ - Controls whether the API should show the original plan when Azure Subscription is not enabled
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Delete the azure subscriptions for the app

*Tags:* `account`

#### Input Parameters
* `azure_subscription_id` - _required_ - The unique ID (UUID) of the azure subscription
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Returns a list of azure subscriptions for the app

*Tags:* `account`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Link azure subscription to an app

*Tags:* `account`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Sets the app avatar

*Tags:* `account`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Deletes the uploaded app avatar

*Tags:* `account`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Returns users of a tenant.<br/>
> Returns all users if no searchTerm param is specified.

*Tags:* `mbaas`

#### Input Parameters
* `AC-Authorization-AAD-Graph` - _optional_ - MSGraph Auth Token
* `searchTerm` - _optional_ - User search term
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Fetch all apple test flight groups

*Tags:* `distribute`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Get mapping of apple app to an existing app in apple store.

*Tags:* `distribute`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Delete mapping of apple app to an existing app in apple store.

*Tags:* `distribute`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Create a mapping for an existing app in apple store for the specified application.

*Tags:* `distribute`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Count of active versions in the time range ordered by version.

*Tags:* `analytics`

#### Input Parameters
* `start` - _required_ - Start date time in data in ISO 8601 date time format.
* `end` - _optional_ - Last date time in data in ISO 8601 date time format.
* `$top` - _optional_ - The maximum number of results to return. (0 will fetch all results)
* `versions` - _optional_
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Count of sessions per device in the time range.

*Tags:* `analytics`

#### Input Parameters
* `start` - _required_ - Start date time in data in ISO 8601 date time format.
* `end` - _optional_ - Last date time in data in ISO 8601 date time format.
* `interval` - _required_ - Size of interval in ISO 8601 duration format. (PnYnMnDTnHnMnS|PnW|P<date>T<time>). The valid durations are 1 day (P1D), 1 week (P1W), and 30 days (P30D).
* `versions` - _optional_
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Gets session duration.

*Tags:* `analytics`

#### Input Parameters
* `start` - _required_ - Start date time in data in ISO 8601 date time format.
* `end` - _optional_ - Last date time in data in ISO 8601 date time format.
* `versions` - _optional_
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Count of sessions in the time range.

*Tags:* `analytics`

#### Input Parameters
* `start` - _required_ - Start date time in data in ISO 8601 date time format.
* `end` - _optional_ - Last date time in data in ISO 8601 date time format.
* `interval` - _required_ - Size of interval in ISO 8601 duration format. (PnYnMnDTnHnMnS|PnW|P<date>T<time>). The valid durations are 1 day (P1D), 1 week (P1W), and 30 days (P30D).
* `versions` - _optional_
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Places in the time range.

*Tags:* `analytics`

#### Input Parameters
* `start` - _required_ - Start date time in data in ISO 8601 date time format.
* `end` - _optional_ - Last date time in data in ISO 8601 date time format.
* `$top` - _optional_ - The maximum number of results to return. (0 will fetch all results)
* `versions` - _optional_
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### OSes in the time range.

*Tags:* `analytics`

#### Input Parameters
* `start` - _required_ - Start date time in data in ISO 8601 date time format.
* `end` - _optional_ - Last date time in data in ISO 8601 date time format.
* `$top` - _optional_ - The maximum number of results to return. (0 will fetch all results)
* `versions` - _optional_
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Models in the time range.

*Tags:* `analytics`

#### Input Parameters
* `start` - _required_ - Start date time in data in ISO 8601 date time format.
* `end` - _optional_ - Last date time in data in ISO 8601 date time format.
* `$top` - _optional_ - The maximum number of results to return. (0 will fetch all results)
* `versions` - _optional_
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Logs received between the specified start time and the current time. The API will return a maximum of 100 logs per call.

*Tags:* `analytics`

#### Input Parameters
* `start` - _optional_ - Start date time in data in ISO 8601 date time format. It must be within the current day in the UTC timezone. The default value is the start time of the current day in UTC timezone.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Languages in the time range.

*Tags:* `analytics`

#### Input Parameters
* `start` - _required_ - Start date time in data in ISO 8601 date time format.
* `end` - _optional_ - Last date time in data in ISO 8601 date time format.
* `$top` - _optional_ - The maximum number of results to return. (0 will fetch all results)
* `versions` - _optional_
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Logs received between the specified start time and the current time. The API will return a maximum of 100 logs per call.

*Tags:* `analytics`

#### Input Parameters
* `start` - _optional_ - Start date time in data in ISO 8601 date time format. It must be within the current day in the UTC timezone. The default value is the start time of the current day in UTC timezone.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Event properties value counts during the time range in descending order.

*Tags:* `analytics`

#### Input Parameters
* `event_name` - _required_ - The id of the event.
* `event_property_name` - _required_ - The id of the event property.
* `start` - _required_ - Start date time in data in ISO 8601 date time format.
* `end` - _optional_ - Last date time in data in ISO 8601 date time format.
* `versions` - _optional_
* `$top` - _optional_ - The number of property values to return. Set to 0 in order to fetch all results available.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Event properties.

*Tags:* `analytics`

#### Input Parameters
* `event_name` - _required_ - The id of the event.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Count of events by interval in the time range.

*Tags:* `analytics`

#### Input Parameters
* `event_name` - _required_ - The id of the event.
* `start` - _required_ - Start date time in data in ISO 8601 date time format.
* `end` - _optional_ - Last date time in data in ISO 8601 date time format.
* `versions` - _optional_
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Count of devices for an event by interval in the time range.

*Tags:* `analytics`

#### Input Parameters
* `event_name` - _required_ - The id of the event.
* `start` - _required_ - Start date time in data in ISO 8601 date time format.
* `end` - _optional_ - Last date time in data in ISO 8601 date time format.
* `versions` - _optional_
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Count of events per session by interval in the time range.

*Tags:* `analytics`

#### Input Parameters
* `event_name` - _required_ - The id of the event.
* `start` - _required_ - Start date time in data in ISO 8601 date time format.
* `end` - _optional_ - Last date time in data in ISO 8601 date time format.
* `versions` - _optional_
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Count of events per device by interval in the time range.

*Tags:* `analytics`

#### Input Parameters
* `event_name` - _required_ - The id of the event.
* `start` - _required_ - Start date time in data in ISO 8601 date time format.
* `end` - _optional_ - Last date time in data in ISO 8601 date time format.
* `versions` - _optional_
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Delete the set of Events with the specified event names.

*Tags:* `analytics`

#### Input Parameters
* `event_name` - _required_ - The id of the event.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Count of active events in the time range ordered by event.

*Tags:* `analytics`

#### Input Parameters
* `start` - _required_ - Start date time in data in ISO 8601 date time format.
* `end` - _optional_ - Last date time in data in ISO 8601 date time format.
* `versions` - _optional_
* `event_name` - _optional_ - To select the specific events.
* `$top` - _optional_ - The maximum number of results to return. (0 will fetch all results)
* `$skip` - _optional_ - The offset (starting at 0) of the first result to return. This parameter along with limit is used to perform pagination.
* `$inlinecount` - _optional_ - Controls whether or not to include a count of all the items across all pages.
    Possible values: allpages, none.
* `$orderby` - _optional_ - controls the sorting order and sorting based on which column
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Delete the set of Events with the specified event names.

*Tags:* `analytics`

#### Input Parameters
* `event_name` - _required_ - The id of the event.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Count of total downloads for the provided distribution releases.

*Tags:* `analytics`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Percentage of crash-free device by day in the time range based on the selected versions. Api will return -1 if crash devices is greater than active devices.

*Tags:* `analytics`

#### Input Parameters
* `start` - _required_ - Start date time in data in ISO 8601 date time format.
* `end` - _optional_ - Last date time in data in ISO 8601 date time format.
* `version` - _required_
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Available for UWP apps only.

> Overall crashes and affected users count of the selected crash group with selected version. Available for UWP apps only.

*Tags:* `analytics`

#### Input Parameters
* `crash_group_id` - _required_ - The id of the crash group.
* `version` - _required_
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Available for UWP apps only.

> Top OSes of the selected crash group with selected version. Available for UWP apps only.

*Tags:* `analytics`

#### Input Parameters
* `crash_group_id` - _required_ - The id of the crash group.
* `version` - _required_
* `$top` - _optional_ - The maximum number of results to return. (0 will fetch all results)
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Available for UWP apps only.

> Top models of the selected crash group with selected version. Available for UWP apps only.

*Tags:* `analytics`

#### Input Parameters
* `crash_group_id` - _required_ - The id of the crash group.
* `version` - _required_
* `$top` - _optional_ - The maximum number of results to return. (0 will fetch all results)
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Available for UWP apps only.

> Count of crashes by day in the time range of the selected crash group with selected version. Available for UWP apps only.

*Tags:* `analytics`

#### Input Parameters
* `crash_group_id` - _required_ - The id of the crash group.
* `version` - _required_
* `start` - _required_ - Start date time in data in ISO 8601 date time format.
* `end` - _optional_ - Last date time in data in ISO 8601 date time format.
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Overall crashes and affected users count of the selected crash groups with selected versions.

*Tags:* `analytics`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Available for UWP apps only.

> Count of crashes by day in the time range based the selected versions. Available for UWP apps only.

*Tags:* `analytics`

#### Input Parameters
* `start` - _required_ - Start date time in data in ISO 8601 date time format.
* `end` - _optional_ - Last date time in data in ISO 8601 date time format.
* `versions` - _optional_
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Returns whether audience definition exists.

*Tags:* `analytics`

#### Input Parameters
* `audience_name` - _required_ - The name of the audience
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Deletes audience definition.

*Tags:* `analytics`

#### Input Parameters
* `audience_name` - _required_ - The name of the audience
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Gets audience definition.

*Tags:* `analytics`

#### Input Parameters
* `audience_name` - _required_ - The name of the audience
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Creates or updates audience definition.

*Tags:* `analytics`

#### Input Parameters
* `audience_name` - _required_ - The name of the audience
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Get list of device property values.

*Tags:* `analytics`

#### Input Parameters
* `property_name` - _required_ - Device property
* `contains` - _optional_ - Contains string
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Get list of device properties.

*Tags:* `analytics`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Get list of custom properties.

*Tags:* `analytics`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Tests audience definition.

*Tags:* `analytics`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Get list of audiences.

*Tags:* `analytics`

#### Input Parameters
* `include_disabled` - _optional_ - Include disabled audience definitions
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Count of active devices by interval in the time range.

*Tags:* `analytics`

#### Input Parameters
* `start` - _required_ - Start date time in data in ISO 8601 date time format.
* `end` - _optional_ - Last date time in data in ISO 8601 date time format.
* `versions` - _optional_
* `app_build` - _required_
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Return a specific app with the given app name which belongs to the given owner.

*Tags:* `account`

#### Input Parameters
* `owner_name` - _required_ - The name of the owner
* `app_name` - _required_ - The name of the application

### Partially updates a single app

*Tags:* `account`

#### Input Parameters
* `app_name` - _required_ - The name of the application
* `owner_name` - _required_ - The name of the owner

### Delete an app

*Tags:* `account`

#### Input Parameters
* `app_name` - _required_ - The name of the application
* `owner_name` - _required_ - The name of the owner

### Creates a new app and returns it to the caller

*Tags:* `account`

### Returns a list of apps

*Tags:* `account`

#### Input Parameters
* `$orderBy` - _optional_ - The name of the attribute by which to order the response by. By default, apps are in order of creation. All results are ordered in ascending order.
    Possible values: display_name, name.

### Delete the api_token object with the specific id

*Tags:* `account`

#### Input Parameters
* `api_token_id` - _required_ - The unique ID (UUID) of the api token

### Returns api tokens for the authenticated user

*Tags:* `account`

### Creates a new API token

*Tags:* `account`

### Lists user data

*Tags:* `test`

### Lists feature flag data

*Tags:* `test`

### Lists account data

*Tags:* `test`

### Lists all the endpoints available for Test account data

*Tags:* `test`

## License

**flow**ground :- Telekom iPaaS / app-center-client-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
