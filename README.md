---
page_type: sample
languages:
- csharp
products:
- azure
description: "The project in this repository was created using Visual Studio 2019. It targets .Net 5.0."
urlFragment: media-services-v3-dotnet-quickstarts
---

# Azure Media Services v3 quickstart starter samples

## NOTE

You can find the latest and most extensive .NET samples in the [Azure Media Services v3](https://github.com/Azure-Samples/media-services-v3-dotnet) repository.

## Overview

The project in this repository targets [.NET 5.0 SDK](https://dotnet.microsoft.com/download). It demonstrates how to encode and publish an asset with Azure Media Services.

The project supports the Azure Media Services v3 quickstarts article:

|Project name|Article|
|---|---|
|EncodeAndStreamFiles.csproj|[Stream files](https://docs.microsoft.com/azure/media-services/latest/stream-files-dotnet-quickstart)|

## Prerequisites

To run samples in this repository, you need:

* Visual Studio 2019 or Visual Studio Code
* An Azure Media Services account. See the steps described in [Create a Media Services account](https://docs.microsoft.com/azure/media-services/latest/create-account-cli-quickstart).
* Create and fill a .env file based on the [sample file](AMSV3Quickstarts/sample.env), or fill the [appsettings.json](AMSV3Quickstarts/EncodeAndStreamFiles/appsettings.json) file. Be sure to copy the API Access details which are in the Azure portal for the AMS account. (Do not change the sample.env file. The .env file will be ignored from commits as it is listed in the .gitignored file.) 

## NuGet packages

The following NuGet packages were added to the project:

|Package|Description|
|---|---|
|Microsoft.Azure.Management.Media|Azure Media Services SDK. <br/>To make sure you are using the latest Azure Media Services package, check [Microsoft.Azure.Management.Media](https://www.nuget.org/packages/Microsoft.Azure.Management.Media).|
|Microsoft.Rest.ClientRuntime.Azure.Authentication|ADAL authentication library for Azure SDK for NET|
|Microsoft.Extensions.Configuration.EnvironmentVariables|Read configuration values from environment variables and local JSON files|
|Microsoft.Extensions.Configuration.Json|Read configuration values from environment variables and local JSON files
|Azure.Storage.Blobs|Blob Storage SDK|

## To run the project in the solution

* Clean and rebuild the solution.
* Add appropriate values to appsettings.json. For more information, see [Access APIs](https://docs.microsoft.com/azure/media-services/latest/access-api-howto).
