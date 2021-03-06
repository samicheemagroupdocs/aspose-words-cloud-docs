---
title: "Split"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /split/
aliases: [/splitting-a-document/]
keywords: ""
description: "Split Word documents. Split DOCX into small PDF, Word files with ease."
weight: 240
---

Aspose provides a powerful API to split Word documents. It's a common document automation task when you need to break a large document into a number of smaller ones to handle them separately.

For example, you must have been in a situation when you have a massive [DOCX](https://docs.fileformat.com/word-processing/docx/) file, requiring urgent team work. In this case, it is pretty necessary to divide a Word document into sub-documents to speed up the collaborative workflow.

Task to split a [DOCX](https://docs.fileformat.com/word-processing/docx/) document by hand with manual copying and pasting may be a long, labor-intensive, sub-optimal approach. Instead, you can improve your efficiency dramatically with this API by breaking Word document into files, while specifying operation parameters as you need.

Using this API you can easily split a [DOC](https://docs.fileformat.com/word-processing/doc/), [DOT](https://docs.fileformat.com/word-processing/dot/), [DOCX](https://docs.fileformat.com/word-processing/docx/), [DOTX](https://docs.fileformat.com/word-processing/dotx/), [RTF](https://docs.fileformat.com/word-processing/rtf/), [ODT](https://docs.fileformat.com/word-processing/odt/), [OTT](https://docs.fileformat.com/word-processing/ott/), [TXT](https://docs.fileformat.com/word-processing/txt/) document and save the results to [DOC](https://docs.fileformat.com/word-processing/doc/), [DOCX](https://docs.fileformat.com/word-processing/docx/), [PDF](https://docs.fileformat.com/pdf/), [ODT](https://docs.fileformat.com/word-processing/odt/), [RTF](https://docs.fileformat.com/word-processing/rtf/), [HTML](https://docs.fileformat.com/web/html/), [JPEG](https://docs.fileformat.com/image/jpeg/), [PNG](https://docs.fileformat.com/Image/png/) and many other file formats.

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Split/SplitDocument) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser. The description of the important parameters of the API is given below:

|Parameter Name|Type|Description|
| :- | :- | :- |
|format|string|If the format is specified, the response contains the conversion data. Please see the table below for valid formats.|
|from|int|The start page number for splitting, if it is not specified, splitting starts from the first page of the document.|
|to|int|The last page number for splitting, if it is not specified, splitting ends at the last page of the document.|
|zipOutput|bool|ZipOutput or not.|

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to split a document
curl -v "https://api.aspose.cloud/v4.0/words/test_doc.docx/split?from=2&to=3&format=pdf" \
-X PUT \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Content-Length: 0" \
-H "Authorization: Bearer <jwt token>"
```
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "SplitResult": {
    "SourceDocument": {
      "Href": "test_doc.docx",
      "Rel": "self"
    },
    "Pages": [
      {
        "Href": "test_doc_page2.pdf",
        "Rel": "page"
      },
      {
        "Href": "test_doc_page3.pdf",
        "Rel": "page"
      }
    ]
  }
}
```

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

### Split DOCX to PDFs

The following code examples demonstrate how to split all pages in a Word document.

{{< nosnippet >}}
{{< tabs tabTotal="9" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="Golang" tabName7="Ruby" tabName8="Android" tabName9="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "SplitAllPagesToNewPDFs.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "SplitAllPagesToNewPDFs.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "SplitAllPagesToNewPDFs.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "SplitAllPagesToNewPDFs.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "SplitAllPagesToNewPDFs.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "SplitAllPagesToNewPDFs.go" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "SplitAllPagesToNewPDFs.rb" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "Aspose_Cloud_Words_SplitAllPagesToNewPDFs.java" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "Aspose_Words_Swift_SplitAllPagesToNewPDFs.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

### Split specific pages to PDFs

The following code examples demonstrate how to split specific pages of a Word document.

{{< nosnippet >}}
{{< tabs tabTotal="9" tabID="5" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="Golang" tabName7="Ruby" tabName8="Android" tabName9="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "SplitSpecificPagesToNewPDFs.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "SplitSpecificPagesToNewPDFs.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "SplitSpecificPagesToNewPDFs.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "SplitSpecificPagesToNewPDFs.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "SplitSpecificPagesToNewPDFs.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "SplitSpecificPagesToNewPDFs.go" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "SplitSpecificPagesToNewPDFs.rb" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "Aspose_Cloud_Words_SplitSpecificPagesToNewPDFs.java" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "Aspose_Words_Swift_SplitSpecificPagesToNewPDFs.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

### Split specific pages to any Supported Format

The following code examples demonstrate how to split a Word document to any format.

{{< nosnippet >}}
{{< tabs tabTotal="9" tabID="6" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="Golang" tabName7="Ruby" tabName8="Android" tabName9="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "SplitSpecificPagesToPNGs.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "SplitSpecificPagesToPNGs.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "SplitSpecificPagesToPNGs.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "SplitSpecificPagesToPNGs.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "SplitSpecificPagesToPNGs.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "SplitSpecificPagesToPNGs.go" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "SplitSpecificPagesToPNGs.rb" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "Aspose_Cloud_Words_SplitSpecificPagesToPNGs.java" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "Aspose_Words_Swift_SplitSpecificPagesToPNGs.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## See also

- Product page description: <a href="https://products.aspose.cloud/words/python/split" target="_blank">Python</a>, <a href="https://products.aspose.cloud/words/net/split" target="_blank">C#</a>, <a href="https://products.aspose.cloud/words/java/split" target="_blank">Java</a>, <a href="https://products.aspose.cloud/words/nodejs/split" target="_blank">Node.js</a>, <a href="https://products.aspose.cloud/words/php/split" target="_blank">PHP</a>, <a href="https://products.aspose.cloud/words/go/split" target="_blank">Go</a>
- <a href="https://products.aspose.app/words/splitter" target="_blank" rel="noopener">Free online splitter app</a>
