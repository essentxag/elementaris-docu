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
| **id** | **UUID**| ID returned by /sbom or /sbom/temporary-report endpoint | [default to null] |

### Return type

[**ReportReply**](../Models/ReportReply.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="temporaryReport"></a>
# **temporaryReport**
> TemporaryReportReply temporaryReport(TemporaryReportRequest)

Analyze SBOM to receive a report

    Only analyze SBOM without uploading

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **TemporaryReportRequest** | [**TemporaryReportRequest**](../Models/TemporaryReportRequest.md)| CycloneDX SBOM to submit | [optional] |

### Return type

[**TemporaryReportReply**](../Models/TemporaryReportReply.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="uploadSbom"></a>
# **uploadSbom**
> SbomReply uploadSbom(SbomRequest)

Upload SBOM

    Upload SBOM for analyzation and notarization.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **SbomRequest** | [**SbomRequest**](../Models/SbomRequest.md)| SBOM to submit | [optional] |

### Return type

[**SbomReply**](../Models/SbomReply.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

