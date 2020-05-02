---
layout: post
title: Creating Azure Functions using Visual Studio
subtitle :
tags: [Azure]
author: Bon
comments : True
---

In this post, I'll be briefly discussing how to create Azure Functions using Visual Studio. If you have no background regarding Functions yet, please go to this [link](https://docs.microsoft.com/en-us/azure/azure-functions/).

Pre-requisite:
-	Visual Studio (of course lol). I used the 2019 Professional version.
-	An existing Azure tenant with Azure Active Directory.

Development:
-	For this post, we are going to do some HTTP requests to Azure AD and retrieve some claims.
- You may refer to my previous [post](https://bonasfvck.github.io/2020/01/10/retrieving-claims-azure-graph-sitecore.html) regarding the retrieval of Azure AD claims using Graph API.
-	You may now follow the step-by-step [docu](https://tutorials.visualstudio.com/first-azure-function/create-app) of Azure Functions.
- Create the codes inside the Function class.
- If you need to use external libraries, do it via NuGet Manager.

Debugging:
-	Build the solution, create a breakpoint, and press F5.
-	A CLI will appear with the generated API URL.
-	Copy and paste the URL in the browser, supply the needed query parameter and start debugging.

API endpoint:
-	Publish your project, check on the docu above.
-	The function will be generated automatically in the Azure Functions blade.
-	Copy the API endpoint from the highlighted below.
-	Paste the endpoint in the browser or use Postman, then supply the needed query parameter. The json string will be retrieved as expected.

Let me know about your experience. :)