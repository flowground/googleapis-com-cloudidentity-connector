# ![LOGO](logo.png) Cloud Identity **flow**ground Connector

## Description

A generated **flow**ground connector for the Cloud Identity API (version v1).

Generated from: https://api.apis.guru/v2/specs/googleapis.com/cloudidentity/v1/swagger.json<br/>
Generated at: 2019-05-23T12:13:05+03:00

## API Description

API for provisioning and managing identity resources.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### List groups within a customer or a domain.

*Tags:* `groups`

#### Input Parameters
* `pageSize` - _optional_ - The default page size is 200 (max 1000) for the BASIC view, and 50
(max 500) for the FULL view.
* `pageToken` - _optional_ - The next_page_token value returned from a previous list request, if any.
* `parent` - _optional_ - `Required`. May be made Optional in the future.
Customer ID to list all groups from.
* `view` - _optional_ - Group resource view to be returned. Defaults to [View.BASIC]().
    Possible values: VIEW_UNSPECIFIED, BASIC, FULL.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Creates a Group.

*Tags:* `groups`

#### Input Parameters
* `$.xgafv` - _optional_ - V1 error format.
    Possible values: 1, 2.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Looks up [resource<br/>
> name](https://cloud.google.com/apis/design/resource_names) of a Group by<br/>
> its EntityKey.

*Tags:* `groups`

#### Input Parameters
* `groupKey.id` - _optional_ - The ID of the entity within the given namespace. The ID must be unique
within its namespace.
* `groupKey.namespace` - _optional_ - Namespaces provide isolation for IDs, so an ID only needs to be unique
within its namespace.

Namespaces are currently only created as part of IdentitySource creation
from Admin Console. A namespace `"identitysources/{identity_source_id}"` is
created corresponding to every Identity Source `identity_source_id`.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Searches for Groups.

*Tags:* `groups`

#### Input Parameters
* `pageSize` - _optional_ - The default page size is 200 (max 1000) for the BASIC view, and 50
(max 500) for the FULL view.
* `pageToken` - _optional_ - The next_page_token value returned from a previous search request, if any.
* `query` - _optional_ - `Required`. Query string for performing search on groups. Users can search
on parent and label attributes of groups.
EXACT match ('==') is supported on parent, and CONTAINS match ('in') is
supported on labels.
* `view` - _optional_ - Group resource view to be returned. Defaults to [View.BASIC]().
    Possible values: VIEW_UNSPECIFIED, BASIC, FULL.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Deletes a Membership.

*Tags:* `groups`

#### Input Parameters
* `name` - _required_ - [Resource name](https://cloud.google.com/apis/design/resource_names) of the
Membership to be deleted.

Format: `groups/{group_id}/memberships/{member_id}`, where `group_id` is
the unique ID assigned to the Group to which Membership belongs to, and
member_id is the unique ID assigned to the member.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Retrieves a Membership.

*Tags:* `groups`

#### Input Parameters
* `name` - _required_ - [Resource name](https://cloud.google.com/apis/design/resource_names) of the
Membership to be retrieved.

Format: `groups/{group_id}/memberships/{member_id}`, where `group_id` is
the unique id assigned to the Group to which Membership belongs to, and
`member_id` is the unique ID assigned to the member.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Updates a Group.

*Tags:* `groups`

#### Input Parameters
* `name` - _required_ - [Resource name](https://cloud.google.com/apis/design/resource_names) of the
Group in the format: `groups/{group_id}`, where group_id is the unique ID
assigned to the Group.

Must be left blank while creating a Group.
* `updateMask` - _optional_ - Editable fields: `display_name`, `description`
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### List Memberships within a Group.

*Tags:* `groups`

#### Input Parameters
* `pageSize` - _optional_ - The default page size is 200 (max 1000) for the BASIC view, and 50
(max 500) for the FULL view.
* `pageToken` - _optional_ - The next_page_token value returned from a previous list request, if any.
* `parent` - _required_ - [Resource name](https://cloud.google.com/apis/design/resource_names) of the
Group to list Memberships within.

Format: `groups/{group_id}`, where `group_id` is the unique ID assigned to
the Group.
* `view` - _optional_ - Membership resource view to be returned. Defaults to View.BASIC.
    Possible values: VIEW_UNSPECIFIED, BASIC, FULL.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Creates a Membership.

*Tags:* `groups`

#### Input Parameters
* `parent` - _required_ - [Resource name](https://cloud.google.com/apis/design/resource_names) of the
Group to create Membership within. Format: `groups/{group_id}`, where
`group_id` is the unique ID assigned to the Group.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Looks up [resource<br/>
> name](https://cloud.google.com/apis/design/resource_names) of a Membership<br/>
> within a Group by member's EntityKey.

*Tags:* `groups`

#### Input Parameters
* `memberKey.id` - _optional_ - The ID of the entity within the given namespace. The ID must be unique
within its namespace.
* `memberKey.namespace` - _optional_ - Namespaces provide isolation for IDs, so an ID only needs to be unique
within its namespace.

Namespaces are currently only created as part of IdentitySource creation
from Admin Console. A namespace `"identitysources/{identity_source_id}"` is
created corresponding to every Identity Source `identity_source_id`.
* `parent` - _required_ - [Resource name](https://cloud.google.com/apis/design/resource_names) of the
Group to lookup Membership within.

Format: `groups/{group_id}`, where `group_id` is the unique ID assigned to
the Group.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

## License

**flow**ground :- Telekom iPaaS / googleapis-com-cloudidentity-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
