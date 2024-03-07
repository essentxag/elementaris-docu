# SbomApi

All URIs are relative to */api/v1*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getSbomReport**](SbomApi.md#getSbomReport) | **GET** /sbom/reports/{id} | Get report of SBOM |
| [**temporaryReport**](SbomApi.md#temporaryReport) | **POST** /sbom/temporary-report | Analyze SBOM to receive a report |
| [**uploadSbom**](SbomApi.md#uploadSbom) | **POST** /sbom | Upload SBOM |


<a name="getSbomReport"></a>
# **getSbomReport**
> ReportReply getSbomReport(id)

Get report of SBOM

    Get the report of a previously analyzed SBOM

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | **String**| ID returned by /sbom or /sbom/temporary-report endpoint | [default to null] |

### Return type

[**ReportReply**](../Models/ReportReply.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="temporaryReport"></a>
# **temporaryReport**
> TemporaryReportReply temporaryReport(body)

Analyze SBOM to receive a report

    Only analyze SBOM without uploading

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **body** | **oas_any_type_not_mapped**| CycloneDX SBOM to submit | [optional] |

### Return type

[**TemporaryReportReply**](../Models/TemporaryReportReply.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="uploadSbom"></a>
# **uploadSbom**
> SbomReply uploadSbom(projectPath, body)

Upload SBOM

    Upload SBOM for analyzation and notarization.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **projectPath** | **String**| Path of the project. | [default to null] |
| **body** | **oas_any_type_not_mapped**| SBOM to submit | [optional] |

### Return type

[**SbomReply**](../Models/SbomReply.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

