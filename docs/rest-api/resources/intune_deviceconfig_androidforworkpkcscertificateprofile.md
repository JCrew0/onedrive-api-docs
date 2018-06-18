﻿# androidForWorkPkcsCertificateProfile resource type

> **Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change. Use of these APIs in production applications is not supported.

> **Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.

Android For Work PKCS certificate profile

Inherits from [androidForWorkCertificateProfileBase](../resources/intune_deviceconfig_androidforworkcertificateprofilebase.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List androidForWorkPkcsCertificateProfiles](../api/intune_deviceconfig_androidforworkpkcscertificateprofile_list.md)|[androidForWorkPkcsCertificateProfile](../resources/intune_deviceconfig_androidforworkpkcscertificateprofile.md) collection|List properties and relationships of the [androidForWorkPkcsCertificateProfile](../resources/intune_deviceconfig_androidforworkpkcscertificateprofile.md) objects.|
|[Get androidForWorkPkcsCertificateProfile](../api/intune_deviceconfig_androidforworkpkcscertificateprofile_get.md)|[androidForWorkPkcsCertificateProfile](../resources/intune_deviceconfig_androidforworkpkcscertificateprofile.md)|Read properties and relationships of the [androidForWorkPkcsCertificateProfile](../resources/intune_deviceconfig_androidforworkpkcscertificateprofile.md) object.|
|[Create androidForWorkPkcsCertificateProfile](../api/intune_deviceconfig_androidforworkpkcscertificateprofile_create.md)|[androidForWorkPkcsCertificateProfile](../resources/intune_deviceconfig_androidforworkpkcscertificateprofile.md)|Create a new [androidForWorkPkcsCertificateProfile](../resources/intune_deviceconfig_androidforworkpkcscertificateprofile.md) object.|
|[Delete androidForWorkPkcsCertificateProfile](../api/intune_deviceconfig_androidforworkpkcscertificateprofile_delete.md)|None|Deletes a [androidForWorkPkcsCertificateProfile](../resources/intune_deviceconfig_androidforworkpkcscertificateprofile.md).|
|[Update androidForWorkPkcsCertificateProfile](../api/intune_deviceconfig_androidforworkpkcscertificateprofile_update.md)|[androidForWorkPkcsCertificateProfile](../resources/intune_deviceconfig_androidforworkpkcscertificateprofile.md)|Update the properties of a [androidForWorkPkcsCertificateProfile](../resources/intune_deviceconfig_androidforworkpkcscertificateprofile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|Key of the entity. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|renewalThresholdPercentage|Int32|Certificate renewal threshold percentage. Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune_deviceconfig_androidforworkcertificateprofilebase.md)|
|subjectNameFormat|[subjectNameFormat](../resources/intune_deviceconfig_subjectnameformat.md)|Certificate Subject Name Format. Inherited from [androidForWorkCertificateProfileBase](../resources/intune_deviceconfig_androidforworkcertificateprofilebase.md). Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.|
|subjectAlternativeNameType|[subjectAlternativeNameType](../resources/intune_deviceconfig_subjectalternativenametype.md)|Certificate Subject Alternative Name Type. Inherited from [androidForWorkCertificateProfileBase](../resources/intune_deviceconfig_androidforworkcertificateprofilebase.md). Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`.|
|certificateValidityPeriodValue|Int32|Value for the Certificate Validity Period. Inherited from [androidForWorkCertificateProfileBase](../resources/intune_deviceconfig_androidforworkcertificateprofilebase.md)|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune_deviceconfig_certificatevalidityperiodscale.md)|Scale for the Certificate Validity Period. Inherited from [androidForWorkCertificateProfileBase](../resources/intune_deviceconfig_androidforworkcertificateprofilebase.md). Possible values are: `days`, `months`, `years`.|
|extendedKeyUsages|[extendedKeyUsage](../resources/intune_deviceconfig_extendedkeyusage.md) collection|Extended Key Usage (EKU) settings. This collection can contain a maximum of 500 elements. Inherited from [androidForWorkCertificateProfileBase](../resources/intune_deviceconfig_androidforworkcertificateprofilebase.md)|
|certificationAuthority|String|PKCS Certification Authority|
|certificationAuthorityName|String|PKCS Certification Authority Name|
|certificateTemplateName|String|PKCS Certificate Template Name|
|subjectAlternativeNameFormatString|String|Custom String that defines the AAD Attribute.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune_deviceconfig_deviceconfigurationgroupassignment.md) collection|The list of group assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) collection|The list of assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) collection|Device configuration installation status by device. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) collection|Device configuration installation status by user. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) collection|Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|rootCertificate|[androidForWorkTrustedRootCertificate](../resources/intune_deviceconfig_androidforworktrustedrootcertificate.md)|Trusted Root Certificate. Inherited from [androidForWorkCertificateProfileBase](../resources/intune_deviceconfig_androidforworkcertificateprofilebase.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkPkcsCertificateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkPkcsCertificateProfile",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "renewalThresholdPercentage": 1024,
  "subjectNameFormat": "String",
  "subjectAlternativeNameType": "String",
  "certificateValidityPeriodValue": 1024,
  "certificateValidityPeriodScale": "String",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "String",
      "objectIdentifier": "String"
    }
  ],
  "certificationAuthority": "String",
  "certificationAuthorityName": "String",
  "certificateTemplateName": "String",
  "subjectAlternativeNameFormatString": "String"
}
```


