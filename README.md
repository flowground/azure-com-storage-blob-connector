# ![LOGO](logo.png) StorageManagementClient **flow**ground Connector

## Description

A generated **flow**ground connector for the StorageManagementClient API (version 2018-07-01).

Generated from: https://api.apis.guru/v2/specs/azure.com/storage-blob/2018-07-01/swagger.json<br/>
Generated at: 2019-06-11T18:14:31+03:00

## API Description

The Azure Storage Management API.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Lists all containers and does not support a prefix like data plane. Also SRP today does not return continuation token.

*Tags:* `BlobContainers`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group within the user's subscription. The name is case insensitive.
* `accountName` - _required_ - The name of the storage account within the specified resource group. Storage account names must be between 3 and 24 characters in length and use numbers and lower-case letters only.
* `api-version` - _required_ - The API version to use for this operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Deletes specified container under its account.

*Tags:* `BlobContainers`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group within the user's subscription. The name is case insensitive.
* `accountName` - _required_ - The name of the storage account within the specified resource group. Storage account names must be between 3 and 24 characters in length and use numbers and lower-case letters only.
* `containerName` - _required_ - The name of the blob container within the specified storage account. Blob container names must be between 3 and 63 characters in length and use numbers, lower-case letters and dash (-) only. Every dash (-) character must be immediately preceded and followed by a letter or number.
* `api-version` - _required_ - The API version to use for this operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Gets properties of a specified container.

*Tags:* `BlobContainers`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group within the user's subscription. The name is case insensitive.
* `accountName` - _required_ - The name of the storage account within the specified resource group. Storage account names must be between 3 and 24 characters in length and use numbers and lower-case letters only.
* `containerName` - _required_ - The name of the blob container within the specified storage account. Blob container names must be between 3 and 63 characters in length and use numbers, lower-case letters and dash (-) only. Every dash (-) character must be immediately preceded and followed by a letter or number.
* `api-version` - _required_ - The API version to use for this operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Updates container properties as specified in request body. Properties not mentioned in the request will be unchanged. Update fails if the specified container doesn't already exist.

*Tags:* `BlobContainers`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group within the user's subscription. The name is case insensitive.
* `accountName` - _required_ - The name of the storage account within the specified resource group. Storage account names must be between 3 and 24 characters in length and use numbers and lower-case letters only.
* `containerName` - _required_ - The name of the blob container within the specified storage account. Blob container names must be between 3 and 63 characters in length and use numbers, lower-case letters and dash (-) only. Every dash (-) character must be immediately preceded and followed by a letter or number.
* `api-version` - _required_ - The API version to use for this operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Creates a new container under the specified account as described by request body. The container resource includes metadata and properties for that container. It does not include a list of the blobs contained by the container.

*Tags:* `BlobContainers`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group within the user's subscription. The name is case insensitive.
* `accountName` - _required_ - The name of the storage account within the specified resource group. Storage account names must be between 3 and 24 characters in length and use numbers and lower-case letters only.
* `containerName` - _required_ - The name of the blob container within the specified storage account. Blob container names must be between 3 and 63 characters in length and use numbers, lower-case letters and dash (-) only. Every dash (-) character must be immediately preceded and followed by a letter or number.
* `api-version` - _required_ - The API version to use for this operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Clears legal hold tags. Clearing the same or non-existent tag results in an idempotent operation. ClearLegalHold clears out only the specified tags in the request.

*Tags:* `BlobContainers`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group within the user's subscription. The name is case insensitive.
* `accountName` - _required_ - The name of the storage account within the specified resource group. Storage account names must be between 3 and 24 characters in length and use numbers and lower-case letters only.
* `containerName` - _required_ - The name of the blob container within the specified storage account. Blob container names must be between 3 and 63 characters in length and use numbers, lower-case letters and dash (-) only. Every dash (-) character must be immediately preceded and followed by a letter or number.
* `api-version` - _required_ - The API version to use for this operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Extends the immutabilityPeriodSinceCreationInDays of a locked immutabilityPolicy. The only action allowed on a Locked policy will be this action. ETag in If-Match is required for this operation.

*Tags:* `BlobContainers`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group within the user's subscription. The name is case insensitive.
* `accountName` - _required_ - The name of the storage account within the specified resource group. Storage account names must be between 3 and 24 characters in length and use numbers and lower-case letters only.
* `containerName` - _required_ - The name of the blob container within the specified storage account. Blob container names must be between 3 and 63 characters in length and use numbers, lower-case letters and dash (-) only. Every dash (-) character must be immediately preceded and followed by a letter or number.
* `api-version` - _required_ - The API version to use for this operation.
* `subscriptionId` - _required_ - The ID of the target subscription.
* `If-Match` - _required_ - The entity state (ETag) version of the immutability policy to update. A value of "*" can be used to apply the operation only if the immutability policy already exists. If omitted, this operation will always be applied.

### Sets the ImmutabilityPolicy to Locked state. The only action allowed on a Locked policy is ExtendImmutabilityPolicy action. ETag in If-Match is required for this operation.

*Tags:* `BlobContainers`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group within the user's subscription. The name is case insensitive.
* `accountName` - _required_ - The name of the storage account within the specified resource group. Storage account names must be between 3 and 24 characters in length and use numbers and lower-case letters only.
* `containerName` - _required_ - The name of the blob container within the specified storage account. Blob container names must be between 3 and 63 characters in length and use numbers, lower-case letters and dash (-) only. Every dash (-) character must be immediately preceded and followed by a letter or number.
* `api-version` - _required_ - The API version to use for this operation.
* `subscriptionId` - _required_ - The ID of the target subscription.
* `If-Match` - _required_ - The entity state (ETag) version of the immutability policy to update. A value of "*" can be used to apply the operation only if the immutability policy already exists. If omitted, this operation will always be applied.

### Aborts an unlocked immutability policy. The response of delete has immutabilityPeriodSinceCreationInDays set to 0. ETag in If-Match is required for this operation. Deleting a locked immutability policy is not allowed, only way is to delete the container after deleting all blobs inside the container.

*Tags:* `BlobContainers`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group within the user's subscription. The name is case insensitive.
* `accountName` - _required_ - The name of the storage account within the specified resource group. Storage account names must be between 3 and 24 characters in length and use numbers and lower-case letters only.
* `containerName` - _required_ - The name of the blob container within the specified storage account. Blob container names must be between 3 and 63 characters in length and use numbers, lower-case letters and dash (-) only. Every dash (-) character must be immediately preceded and followed by a letter or number.
* `immutabilityPolicyName` - _required_ - The name of the blob container immutabilityPolicy within the specified storage account. ImmutabilityPolicy Name must be 'default'
    Possible values: default.
* `api-version` - _required_ - The API version to use for this operation.
* `subscriptionId` - _required_ - The ID of the target subscription.
* `If-Match` - _required_ - The entity state (ETag) version of the immutability policy to update. A value of "*" can be used to apply the operation only if the immutability policy already exists. If omitted, this operation will always be applied.

### Gets the existing immutability policy along with the corresponding ETag in response headers and body.

*Tags:* `BlobContainers`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group within the user's subscription. The name is case insensitive.
* `accountName` - _required_ - The name of the storage account within the specified resource group. Storage account names must be between 3 and 24 characters in length and use numbers and lower-case letters only.
* `containerName` - _required_ - The name of the blob container within the specified storage account. Blob container names must be between 3 and 63 characters in length and use numbers, lower-case letters and dash (-) only. Every dash (-) character must be immediately preceded and followed by a letter or number.
* `immutabilityPolicyName` - _required_ - The name of the blob container immutabilityPolicy within the specified storage account. ImmutabilityPolicy Name must be 'default'
    Possible values: default.
* `api-version` - _required_ - The API version to use for this operation.
* `subscriptionId` - _required_ - The ID of the target subscription.
* `If-Match` - _optional_ - The entity state (ETag) version of the immutability policy to update. A value of "*" can be used to apply the operation only if the immutability policy already exists. If omitted, this operation will always be applied.

### Creates or updates an unlocked immutability policy. ETag in If-Match is honored if given but not required for this operation.

*Tags:* `BlobContainers`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group within the user's subscription. The name is case insensitive.
* `accountName` - _required_ - The name of the storage account within the specified resource group. Storage account names must be between 3 and 24 characters in length and use numbers and lower-case letters only.
* `containerName` - _required_ - The name of the blob container within the specified storage account. Blob container names must be between 3 and 63 characters in length and use numbers, lower-case letters and dash (-) only. Every dash (-) character must be immediately preceded and followed by a letter or number.
* `immutabilityPolicyName` - _required_ - The name of the blob container immutabilityPolicy within the specified storage account. ImmutabilityPolicy Name must be 'default'
    Possible values: default.
* `api-version` - _required_ - The API version to use for this operation.
* `subscriptionId` - _required_ - The ID of the target subscription.
* `If-Match` - _optional_ - The entity state (ETag) version of the immutability policy to update. A value of "*" can be used to apply the operation only if the immutability policy already exists. If omitted, this operation will always be applied.

### Sets legal hold tags. Setting the same tag results in an idempotent operation. SetLegalHold follows an append pattern and does not clear out the existing tags that are not specified in the request.

*Tags:* `BlobContainers`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group within the user's subscription. The name is case insensitive.
* `accountName` - _required_ - The name of the storage account within the specified resource group. Storage account names must be between 3 and 24 characters in length and use numbers and lower-case letters only.
* `containerName` - _required_ - The name of the blob container within the specified storage account. Blob container names must be between 3 and 63 characters in length and use numbers, lower-case letters and dash (-) only. Every dash (-) character must be immediately preceded and followed by a letter or number.
* `api-version` - _required_ - The API version to use for this operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Gets the properties of a storage account's Blob service, including properties for Storage Analytics and CORS (Cross-Origin Resource Sharing) rules.

*Tags:* `BlobService`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group within the user's subscription. The name is case insensitive.
* `accountName` - _required_ - The name of the storage account within the specified resource group. Storage account names must be between 3 and 24 characters in length and use numbers and lower-case letters only.
* `api-version` - _required_ - The API version to use for this operation.
* `subscriptionId` - _required_ - The ID of the target subscription.
* `BlobServicesName` - _required_ - The name of the blob Service within the specified storage account. Blob Service Name must be 'default'
    Possible values: default.

### Sets the properties of a storage account's Blob service, including properties for Storage Analytics and CORS (Cross-Origin Resource Sharing) rules.

*Tags:* `BlobService`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group within the user's subscription. The name is case insensitive.
* `accountName` - _required_ - The name of the storage account within the specified resource group. Storage account names must be between 3 and 24 characters in length and use numbers and lower-case letters only.
* `api-version` - _required_ - The API version to use for this operation.
* `subscriptionId` - _required_ - The ID of the target subscription.
* `BlobServicesName` - _required_ - The name of the blob Service within the specified storage account. Blob Service Name must be 'default'
    Possible values: default.

## License

**flow**ground :- Telekom iPaaS / azure-com-storage-blob-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
