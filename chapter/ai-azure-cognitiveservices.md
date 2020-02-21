# :o: Cognitive Services on Azure sp20-516-243 David Drummond

## Introduction

Cognitive services on Azure provides AI technologies to those with little AI understanding. It is the umbrella service for all of the pretrained models in Azure's library. These services provide valuable resources for those who need vanilla AI service applications without much custom tuning. They provide API or SDK plugins for REST API, Python, .NET, Node.js,and Go. With this broad spectrum of native and plugin application, it gives developers relevant tools to incorporate these services into their applications. [[Documentation](https://docs.microsoft.com/en-us/azure/cognitive-services/face/index)] 

## Applications

As cognitive services is an umbrella service, there are different categories of developer tools within this service. This includes decision tools, language tools, speech tools, vision tools, and search tools. Not all tools are available in all regions. [[Documentation](<https://azure.microsoft.com/en-us/global-infrastructure/services/?products=all>)]. 
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
|Standard	|10 TPS	                        |Moderate, Review |	0-1M transactions - $1 per 1,000 transactions   |
|         |                               |                 |1M-5M transactions - $0.75 per 1,000 transactions|
|         |                               |                 |5M-10M transactions - $0.60 per 1,000 transactions|
|         |                               |                 |10M+ transactions - $0.40 per 1,000 transactions  |

<https://azure.microsoft.com/en-us/services/cognitive-services/content-moderator/>

#### Personalizer

Personalizer is a ready to use, SDK for user recomendations on end user expereinces. This service has limited server rollout. 

The algorithm works by the developer assigning user actions to a algorithmic reward system. If the computer correctly identifies the users action, it is rewarded, else it recieves not reward and adjusts the algorithm. 

<https://docs.microsoft.com/en-us/azure/cognitive-services/personalizer/what-is-personalizer>

<https://azure.microsoft.com/en-us/services/cognitive-services/personalizer/>

### Language

#### Immersive Reader

Immersive reader is a preview only service to add AI text to speech integration for accessibility services. In preview, this feature is free and pricing out of preview is unavailable. The SDK packs for this projects are limited to Swift, node.js, and ASP.NET Core. The main features of immersive reader are text to speech, focused reading windows, visual reading cues, and syllable-word breakdown. 

<https://docs.microsoft.com/en-us/azure/cognitive-services/immersive-reader/>

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



