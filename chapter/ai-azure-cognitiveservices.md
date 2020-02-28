# :o: Cognitive Services on Azure sp20-516-243 David Drummond

## Introduction

Cognitive services on Azure provides AI technologies to those with little AI understanding. It is the umbrella service for all of the pretrained models in Azure's library. These services provide valuable resources for those who need vanilla AI service applications without much custom tuning. They provide API or SDK plugins for REST API, Python, .NET, Node.js,and Go. With this broad spectrum of native and plugin application, it gives developers relevant tools to incorporate these services into their applications. [[Documentation](https://docs.microsoft.com/en-us/azure/cognitive-services/face/index)] 

## Applications

As cognitive services is an umbrella service, there are different categories of developer tools within this service. This includes decision tools, language tools, speech tools, and vision tools. Not all tools are available in all regions. [[Documentation](<https://azure.microsoft.com/en-us/global-infrastructure/services/?products=all>)]. 

### Decision

Decision tools enable stakeholders to automate data analysis for a variety of applications including anomoly detection, content moderation, and personalizing. This can provide service for both end-user and developer to scale businesses and automate menial work.  

#### Anomoly Detector

Anomoly detector is a decision feature that provides automated detection of outstanding data patterns. Specifically, this tool works to monitor any time-series data. This feature is in preview phase, therefore access is limited. 

Azure suggests this tool can be applied to business metrics, IoT data stream, or any time timestamps are applied to data. The algorithm looks for seasonality, spikes, and dips in the data. [[Video](<https://channel9.msdn.com/Shows/AI-Show/Introducing-Azure-Anomaly-Detector?WT.mc_id=ai-c9-niner>)] This tool has been used by Microsoft in their Microsoft 365 product management for several years and recently made the tool available to developers. 

The anomoly service [API](<https://docs.microsoft.com/en-us/azure/cognitive-services/anomaly-detector/>) kits are accessible through the Azure documentation.  


|Account                  |INSTANCE	PRICE                    |
|---                      |---                               |
|Free- Web/Container      |	20000 transactions free per month|
|Standard - Web/Container |	$0.157 per 1,000 transactions    |

<https://azure.microsoft.com/en-us/services/cognitive-services/anomaly-detector/>

#### Content Moderator

Content moderator serves as a gatekeeper for content on user generated content. It will detect offensive content in text, videos, and images. Most, but not all servers have this feature installed. This feature is most often used with user generated content platforms. This tool scans uploaded images, texts, and videos and tags potentiallly objectionable content. This content can then be passed to a moderator for human review. The human review updates the model with his or her feedback 

|Account  |	Transactions per Second (TPS)	| Features        |	Price                                           |
|---      |---                            |---              |---                                              |
|Free     |	1 TPS	                        | Moderate, Review| N/A                                             |
|Standard	|10 TPS	                        |Moderate, Review |	0-1M transactions - $1 per 1,000 transactions <br> 1M-5M transactions - $0.75 per 1,000 transactions <br> 5M-10M transactions - $0.60 per 1,000 transactions <br> 10M+ transactions - $0.40 per 1,000 transactions|

<https://azure.microsoft.com/en-us/services/cognitive-services/content-moderator/>

#### Personalizer

Personalizer is a ready to use, SDK for user recomendations on end user expereinces. This service has limited server rollout. 

The algorithm works by the developer assigning user actions to a algorithmic reward system. If the computer correctly identifies the users action, it is rewarded, else it recieves not reward and adjusts the algorithm. 

|Account|Price|Storage|
|---|---|---|
|Free|50,000 transactions free /month| 10 GB|
|Paid|First 1M transactions $1 per 1000 transactions <br> Next 9M transaction $0.35 per 1000 transactions <br> Next 90M transaction $0.20 per 1000 transactions <br> Above 100M transactions $0.05 per 1000 transactions |10 GB/1M transactions/month|

||Above 100M transactions $0.05 per 1000 transactions||

<https://docs.microsoft.com/en-us/azure/cognitive-services/personalizer/what-is-personalizer>

<https://azure.microsoft.com/en-us/services/cognitive-services/personalizer/>

### Language

The language application package aims to add natural language processing tools to developers in the form of API and SDK. 

#### Immersive Reader

Immersive reader is a preview only service to add AI text to speech integration for accessibility services. In preview, this feature is free and pricing out of preview is unavailable. The SDK packs for this projects are limited to Swift, node.js, and ASP.NET Core. The main features of immersive reader are text to speech, focused reading windows, visual reading cues, and syllable-word breakdown. 

<https://docs.microsoft.com/en-us/azure/cognitive-services/immersive-reader/>

<https://azure.microsoft.com/en-us/services/cognitive-services/immersive-reader/>

#### Language Understanding

Language Understanding is a pretrained natural language processor. It is available through SDK using C#, Python, and JavaScript. It is additionally available using REST in all REST compatible languages. Free versions of language understanding can process typed language; whereas, the paid version can process both typed and spoken language. Language understanding can be applied to bot services or IoT control. 

|INSTANCE|TRANSACTIONS PER SECOND (TPS)|FEATURES|PRICE|
|---     |---                          |---     |---|
|Free Web/Container|	5 TPS |	Text Requests|10,000 transactions free per month|
|Standard|50 TPS|Text Requests|$1.50 per 1000 transactions|
|||Speech Requests|$5.50 per 1000 transactions|

<https://azure.microsoft.com/en-us/services/cognitive-services/language-understanding-intelligent-service/>

#### QnA Maker

QnA Maker uses Knowledge base databases to create a chat bot. It can be customized to different levels of formality. It allows for additional processes to be added over time. It supports C#, Python, and JavaScript. For knowledge base integreation it supports cURL and Postman.

|INSTANCE|TRANSACTIONS PER SECOND (TPS)|LIMITATIONS|PRICE|
|---     |---                          |---     |---|
|Free Web/Container|	3 TPS |	Up to 1MB each document <br> Up to 1MB each document <br> Up to 100 transactions per minute <br> Up to 50,000 transactions per month|3 managed documents free per month|
|Standard|3 TPS|Up to 100 transactions per minute|$10 for unlimited managed documents|

<https://docs.microsoft.com/en-us/azure/cognitive-services/QnAMaker/quickstarts/get-answer-from-knowledge-base-using-url-tool?pivots=url-test-tool-curl>

<https://azure.microsoft.com/en-us/services/cognitive-services/qna-maker/>

#### Text Analytics

Text analytics aims to provide broad range text analytic service in SDK packaging. The key features are sentiment analysis, key phrases extraction, named entities extraction and language determination. There is SDK available for C#, Python, Node.js, Go, and Ruby. It provides easy integration to Power BI and Flask. 

|INSTANCE|FEATURES|PRICE|
|---|---|---|
|Free|Sentiment Analysis <br> Key Phrase Extraction <br> Language Detection <br> Named Entity Recognition (not available in Container)| N/A|
|Standard|Sentiment Analysis <br> Key Phrase Extraction <br> Language Detection <br> Named Entity Recognition (not available in Container)|0-500,000 text records — $2 per 1,000 text records <br> 0.5M-2.5M text records — $1 per 1,000 text records <br> 2.5M-10.0M text records — $0.50 per 1,000 text records <br> 10M+ text records — $0.25 per 1,000 text records |
|S0 |Sentiment Analysis <br> Key Phrase Extraction <br> Language Detection <br> Named Entity Recognition | $74.71/month <br> Up to 25,000 transactions per month <br> <br> Overage: $3 per 1,000 transactions |
|S1 |Sentiment Analysis <br> Key Phrase Extraction <br> Language Detection <br> Named Entity Recognition | $249.86/month <br> Up to 100,000 transactions per month <br> <br> Overage: $2.50 per 1,000 transactions |
|S2 |Sentiment Analysis <br> Key Phrase Extraction <br> Language Detection <br> Named Entity Recognition | $999.75/month <br> Up to 500,000 transactions per month <br> <br> Overage: $2 per 1,000 transactions |
|S3 |Sentiment Analysis <br> Key Phrase Extraction <br> Language Detection <br> Named Entity Recognition | $2,499.84/month <br> Up to 2,500,000 transactions per month <br> <br> Overage: $1 per 1,000 transactions |
|S4 |Sentiment Analysis <br> Key Phrase Extraction <br> Language Detection <br> Named Entity Recognition | $4999.99/month <br> Up to 10,000,000 transactions per month <br> <br> Overage: $0.50 per 1,000 transactions |

<https://azure.microsoft.com/en-us/services/cognitive-services/text-analytics/>

#### Translator Text

The translator text API provides neural translator services for developer integration. It is available in C# and REST API. Azure marketing tools indicate that it is useful for increasing research text data, detecting input language, bilingual dictionary tools, on device translation, and custom trained translation. 

|INSTANCE|FEATURES|PRICE|
|---|---|---|
|Free|Standard Translation <br>    -Text Translation <br>    -Language Detection <br>    -Bilingual Dictionary <br>    -Transliteration <br> Custom Translation <br>    -Training| 2M Characters Free|
|S1|Standard Translation <br>    -Text Translation <br>    -Language Detection <br>    -Bilingual Dictionary <br>    -Transliteration <br> Custom Translation <br>    -Training <br>  -Translation <br> -Custom model hosting| Standard <br>  - $10 per million characters <br> <br> <br> Custom <br> -$40 per million chars of custom translation <br> -$10 per million source + target chars of training data (max. $300/training) <br> -$10 per hosted custom translation model per region, per month|

<https://azure.microsoft.com/en-us/services/cognitive-services/translator-text-api/>

### Speech

Speech packages adds additional natural language processing tools to developers for spoken language. 

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

