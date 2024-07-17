# Documentation for Elementaris Service

<a name="documentation-for-api-endpoints"></a>
## Documentation for API Endpoints

All URIs are relative to */api/v1*

| Class | Method | HTTP request | Description |
|------------ | ------------- | ------------- | -------------|
| *SbomApi* | [**getSbom**](Apis/SbomApi.md#getsbom) | **GET** /sbom | Get SBOM |
*SbomApi* | [**getSbomReport**](Apis/SbomApi.md#getsbomreport) | **GET** /sbom/reports/{id} | Get report of SBOM |
*SbomApi* | [**getTrustLevel**](Apis/SbomApi.md#gettrustlevel) | **GET** /sbom/trustlevels | Get trustlevel of analyzed SBOM |
*SbomApi* | [**temporaryReport**](Apis/SbomApi.md#temporaryreport) | **POST** /sbom/temporary-report | Analyze SBOM to receive a report |
*SbomApi* | [**uploadSbom**](Apis/SbomApi.md#uploadsbom) | **POST** /sbom | Upload SBOM |


<a name="documentation-for-models"></a>
## Documentation for Models

 - [ErrorReply](./Models/ErrorReply.md)
 - [ReportReply](./Models/ReportReply.md)
 - [SbomReply](./Models/SbomReply.md)
 - [SbomReport](./Models/SbomReport.md)
 - [SbomVulnerability](./Models/SbomVulnerability.md)
 - [SbomVulnerabilityIssue](./Models/SbomVulnerabilityIssue.md)
 - [TemporaryReportReply](./Models/TemporaryReportReply.md)
 - [TrustLevel](./Models/TrustLevel.md)
 - [TrustlevelReply](./Models/TrustlevelReply.md)


<a name="documentation-for-authorization"></a>
## Documentation for Authorization

<a name="ApiKeyAuth"></a>
### ApiKeyAuth

- **Type**: API key
- **API key parameter name**: X-API-Key
- **Location**: HTTP header

<a name="api_key"></a>
### api_key

- **Type**: API key
- **API key parameter name**: Authorization
- **Location**: HTTP header

