# Cheminee::DefaultApi

All URIs are relative to *http://localhost:3000/api*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**standardize_post**](DefaultApi.md#standardize_post) | **POST** /standardize |  |


## standardize_post

> <Array<Smile>> standardize_post(smile)



### Examples

```ruby
require 'time'
require 'cheminee'

api_instance = Cheminee::DefaultApi.new
smile = [Cheminee::Smile.new({smile: 'smile_example'})] # Array<Smile> | 

begin
  
  result = api_instance.standardize_post(smile)
  p result
rescue Cheminee::ApiError => e
  puts "Error when calling DefaultApi->standardize_post: #{e}"
end
```

#### Using the standardize_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<Smile>>, Integer, Hash)> standardize_post_with_http_info(smile)

```ruby
begin
  
  data, status_code, headers = api_instance.standardize_post_with_http_info(smile)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<Smile>>
rescue Cheminee::ApiError => e
  puts "Error when calling DefaultApi->standardize_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **smile** | [**Array&lt;Smile&gt;**](Smile.md) |  |  |

### Return type

[**Array&lt;Smile&gt;**](Smile.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

