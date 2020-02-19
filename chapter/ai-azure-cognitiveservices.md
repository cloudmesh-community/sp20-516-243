# :o: Cognitive Services on Azure sp20-516-243 David Drummond

## Introduction

Cognitive services on Azure provides AI technologies to those with little AI understanding. It is the umbrella service for all of the pretrained models in Azure's library. These services provide valuable resources for those who need vanilla AI service applications without much custom tuning. They provide API or SDK plugins for REST API, Python, .NET, Node.js,and Go. With this broad spectrum of native and plugin application, it gives developers relevant tools to incorporate these services into their applications. [[Documentation](https://docs.microsoft.com/en-us/azure/cognitive-services/face/index)] 

## Applications

As cognitive services is an umbrella service, there are different categories of developer tools within this service. This includes decision tools, language tools, speech tools, vision tools, and search tools. 

### Decision

Decision tools enable stakeholders to automate data analysis for a variety of applications including anomoly detection, content moderation, and personalizing. This can provide service for both end-user and developer to scale businesses and automate menial work. Not all tools are available in all regions. [[Documentation](<https://azure.microsoft.com/en-us/global-infrastructure/services/?products=all>)]. In each description, availablility of the service is provided. 

#### Anomoly Detector

Anomoly detector is a decision feature that provides automated detection of outstanding data patterns. Specifically, this tool works to monitor any time-series data. This feature is in preview phase, therefore access is limited. Specifically, this feature is only available in East Asia,	Southeast Asia, Australia East, Canada Central, North Europe, UK South,	Central US,	East US, East US 2, and South Central US server regions are loaded with the preview state.

Azure suggests this tool can be applied to business metrics, IoT data stream, or any time timestamps are applied to data. The algorithm looks for seasonality, spikes, and dips in the data. [[Video](<https://channel9.msdn.com/Shows/AI-Show/Introducing-Azure-Anomaly-Detector?WT.mc_id=ai-c9-niner>)] This tool has been used by Microsoft in their Microsoft 365 product management for several years and recently made the tool available to developers. 

The anomoly service [API](<https://docs.microsoft.com/en-us/azure/cognitive-services/anomaly-detector/>) kits are accessible through the Azure documentation.  

<https://azure.microsoft.com/en-us/services/cognitive-services/anomaly-detector/>

#### Content Moderator

Content moderator serves as a gatekeeper for content on user generated content. It will detect offensive content in text, videos, and images. Most, but not all servers have this feature installed. Those regions eligible are South Africa North, East Asia, Southeast Asia, Australia East, US Gov Virginia, Brazil South, Canada Central, China East 2, China North, North Europe, West Europe, France Central, Central India, Japan East, Japan West, Korea Central, UK South, Central US, East US, East US 2, North Central US, South Central US, West Central US, West US, and West US 2. This feature is most often used with user generated content platforms. This tool scans uploaded images, texts, and videos and tags potentiallly objectionable content. This content can then be passed to a moderator for human review. The human review updates the model with his or her feedback 

<https://azure.microsoft.com/en-us/services/cognitive-services/content-moderator/>

#### Personalizer

Personalizer is a ready to use, SDK for user recomendations on end user expereinces. This service is only available in the East Asia, Southeast Asia, Canada Central, North Europe, West Europe, UK South, UK West, Central US, East US, Australia East, West US 2 region servers. 

The algorithm works by the developer assigning user actions to a algorithmic reward system. If the computer correctly identifies the users action, it is rewarded, else it recieves not reward and adjusts the algorithm. 

<https://docs.microsoft.com/en-us/azure/cognitive-services/personalizer/what-is-personalizer>

<https://azure.microsoft.com/en-us/services/cognitive-services/personalizer/>

### Language

#### Immersive Reader

<https://azure.microsoft.com/en-us/services/cognitive-services/immersive-reader/>

#### Language Understanding

<https://azure.microsoft.com/en-us/services/cognitive-services/language-understanding-intelligent-service/>

#### QnA Maker

<https://azure.microsoft.com/en-us/services/cognitive-services/qna-maker/>

#### Text Analytics

<https://azure.microsoft.com/en-us/services/cognitive-services/text-analytics/>

#### Translator Text

<https://azure.microsoft.com/en-us/services/cognitive-services/translator-text-api/>

### Speech

#### Speech to Text

<https://azure.microsoft.com/en-us/services/cognitive-services/speech-to-text/>

#### Text to Speech

<https://azure.microsoft.com/en-us/services/cognitive-services/text-to-speech/>)

#### Speech Translation

<https://azure.microsoft.com/en-us/services/cognitive-services/speech-translation/>

#### Speaker Recognition

<https://azure.microsoft.com/en-us/services/cognitive-services/speaker-recognition/>)

### Vision

#### Computer Vision

<https://azure.microsoft.com/en-us/services/cognitive-services/computer-vision/>

#### Custom Vision

<https://azure.microsoft.com/en-us/services/cognitive-services/custom-vision-service/>

#### Face

<https://azure.microsoft.com/en-us/services/cognitive-services/face/>

#### Form Recognizer

<https://azure.microsoft.com/en-us/services/cognitive-services/form-recognizer/>

#### Ink Recognizer

<https://azure.microsoft.com/en-us/services/cognitive-services/ink-recognizer/>

#### Video Indexer

<https://azure.microsoft.com/en-us/services/media-services/video-indexer/>

### Search

#### Bing Autosuggest

<https://azure.microsoft.com/en-us/services/cognitive-services/autosuggest/>

#### Bing Custom Search

<https://azure.microsoft.com/en-us/services/cognitive-services/bing-custom-search/>

#### Bing Entity Search

<https://azure.microsoft.com/en-us/services/cognitive-services/bing-entity-search-api/>

#### Bing Image Search

<https://azure.microsoft.com/en-us/services/cognitive-services/bing-image-search-api/>

#### Bing News Search

<https://azure.microsoft.com/en-us/services/cognitive-services/bing-news-search-api/>

#### Bing Spell Check

<https://azure.microsoft.com/en-us/services/cognitive-services/spell-check/>

#### Bing Video Search

<https://azure.microsoft.com/en-us/services/cognitive-services/bing-video-search-api/>

#### Bing Visual Search

<https://azure.microsoft.com/en-us/services/cognitive-services/bing-visual-search/>

#### Bing Web Search

<https://azure.microsoft.com/en-us/services/cognitive-services/bing-web-search-api/>



