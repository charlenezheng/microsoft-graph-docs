---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentResource educationAssignmentResource = new EducationAssignmentResource();
educationAssignmentResource.distributeForStudentWork = false;
EducationLinkResource resource = new EducationLinkResource();
resource.displayName = "Bing";
resource.link = "https://www.bing.com";
educationAssignmentResource.resource = resource;

graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignments("ad8afb28-c138-4ad7-b7f5-a6986c2655a8").resources()
	.buildRequest()
	.post(educationAssignmentResource);

```