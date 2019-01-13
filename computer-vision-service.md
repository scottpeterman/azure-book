# Computer vision service

> WHY Cog Services: You need to decide whether to build or buy a solution. Building a sophisticated image processing and analysis engine is costly. One alternative is to use the Computer Vision API from Microsoft. 
We will do the following

- **Create** a Cognitive Services account.
- **Get** information about the visual content found in an image.
- **Generate** a thumbnail of an image.
- **Detect** and extract printed text from an image.
- **Detect** and extract handwritten text from an image.

## Calling the API

- get an API key
- make a POST call to the API
- parse the JSON response

Format of the URL

```
region.api.cognitive.microsoft.com/vision/v2.0/resource/[parameters]
```

- **region** - the region where you created the account, for example, westus.
- **resource** - the Computer Vision resource you are calling such as 
- **analyze**, describe, generateThumbnail, ocr, models, recognizeText, tag.

## Create a Coginitive Service account

