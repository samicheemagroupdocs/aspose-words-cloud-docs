---
title: "Get Document Statistics"
type: docs
url: /get-document-statistics/
aliases: [/get-document-statistics/]
weight: 70
---

This REST API allows you to get statistical data on the document. The request parameters are the following:

|Parameter Name|Type|Query String/HTTPBody|Description|
| :- | :- | :- | :- |
|includeComments|bool|Query String: includeComments=true|Support including/excluding comments from the WordCount. The default value is "false".|
|includeFootnotes|bool|Query String: includeFootnotes=true|Support including/excluding footnotes from the WordCount. The default value is "false".|
|includeTextInShapes|bool|Query String: includeTextInShapes=true|Support including/excluding shape's text from the WordCount. The default value is "false".|

## REST API’s Resources

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Statistics/GetDocumentStatistics) lets you call this REST API directly from a browser.

## cURL Example

The following are a few examples of using cURL:

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```JAVA
# Please get your App_Key and App_SID credentials from https://dashboard.aspose.cloud/#/apps.
# Place App_Key in "client_secret" and App_SID in "client_id" argument.
curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

# cURL example to get the statistical data of the document
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/statistics" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

{{< /tab >}}
{{< tab tabNum="2" >}}

```JAVA
{
  "StatData": {
    "WordCount": 24,
    "ParagraphCount": 5,
    "PageCount": 3,
    "FootnotesStatData": {
      "WordCount": 0,
      "ParagraphCount": 0
    },
    "PageStatData": [
      {
        "PageNumber": 1,
        "WordCount": 4,
        "ParagraphCount": 2,
        "FootnotesStatData": null
      },
      {
        "PageNumber": 2,
        "WordCount": 9,
        "ParagraphCount": 1,
        "FootnotesStatData": null
      },
      {
        "PageNumber": 3,
        "WordCount": 11,
        "ParagraphCount": 2,
        "FootnotesStatData": null
      }
    ]
  },
  "DocumentLink": {
    "Href": "test_multi_pages.docx",
    "Rel": "self",
    "Type": null,
    "Title": null
  },
  "Code": 200,
  "Status": "OK"
}
```

{{< /tab >}}
{{< /tabs >}}

## Boost the Development Process with Aspose Words Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

A set of short code examples, demonstrating how to use this REST API with various SDKs, is presented below:

{{< tabs tabTotal="8" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetDocumentStatistics.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetDocumentStatistics.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "document_statistics.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "get_document_statistics.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "getDocumentStatistics.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetDocumentStatistics.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetDocumentStatistics.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetDocumentStatistics.go" >}}
{{< /tab >}}
{{< /tabs >}}