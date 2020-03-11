# Cognitive Services on Azure sp20-516-243 David Drummond

## Introduction

Cognitive services on Azure provides AI technologies to those with little AI understanding. It is the umbrella service for all of the pretrained models in Azure's library. These services provide valuable resources for those who need vanilla AI service applications without much custom tuning. With a broad spectrum of native and plugin application, it gives developers relevant tools to incorporate these services into their applications. [@cognitve-intro-sp20-516-243]

## Applications

As cognitive services is an umbrella service, there are different categories of developer tools within this service. This includes decision tools, language tools, speech tools, and vision tools. Not all tools are available in all regions. [@cognitve-product-availability-sp20-516-243]. 

### Decision

Decision tools enable stakeholders to automate data analysis for a variety of applications including anomaly detection, content moderation, and personalizing. This can provide service for both end-user and developer to scale businesses and automate menial work.  

#### Anomaly Detector

Anomaly detector is a decision feature that provides automated detection of outstanding data patterns [@cognitve-anomaly-overview-sp20-516-243]. Specifically, this tool works to monitor any time-series data. This feature is in preview phase, therefore access is limited. 

Azure suggests this tool can be applied to business metrics, IoT data stream, or any time timestamps are applied to data. The algorithm looks for seasonality, spikes, and dips in the data. [@cognitve-anomaly-video-sp20-516-243] This tool has been used by Microsoft in their Microsoft 365 product management for several years and recently made the tool available to developers. 

The anomaly service development kits are accessible through the Azure documentation [@cognitve-anomaly-api-sp20-516-243].  


|Account                  |Price [@cognitve-anomaly-pricing-sp20-516-243]|
|---                      |---                               |
|Free- Web/Container      |	20000 transactions free per month|
|Standard - Web/Container |	$0.157 per 1,000 transactions    |

#### Content Moderator

Content moderator serves as a gatekeeper for content on user generated content. It will detect offensive content in text, videos, and images. Most, but not all servers have this feature installed. This feature is most often used with user generated content platforms. This tool scans uploaded images, texts, and videos and tags potentiallly objectionable content. This content can then be passed to a moderator for human review. The human review updates the model with his or her feedback [@cognitve-moderator-overview-sp20-516-243].

|Account  |	Transactions per Second (TPS)	| Features        |	Price [@cognitve-moderator-pricing-sp20-516-243]|
|---      |---                            |---              |---                 |
|Free     |	1 TPS	                        | Moderate, Review| N/A                |
|         |                               |                 |                    |
|Standard	|10 TPS	                        |Moderate, Review |	0-1M transactions - $1 per 1,000 transactions|
|         |                              |                  |1M-5M transactions - $0.75 per 1,000 transactions|
|         |                              |                  |5M-10M transactions - $0.60 per 1,000 transactions|
|         |                              |                  |10M+ transactions - $0.40 per 1,000 transactions|

#### Personalizer

Personalizer is a ready to use, SDK for user recomendations on end user expereinces [cognitve-personalizer-overview-sp20-516-243]. This service has limited server rollout. 

The algorithm works by the developer assigning user actions to a algorithmic reward system. If the computer correctly identifies the users action, it is rewarded, else it recieves not reward and adjusts the algorithm.[] 

|Account|Price [@cognitve-personalizer-pricing-sp20-516-243]|Storage|
|---|---|---|
|Free|50,000 transactions free /month               | 10 GB                     |
|     |                                              |                          |
|Paid|First 1M transactions $1 per 1000 transactions| 0 GB/1M transactions/month|
|    |Next 9M transaction $0.35 per 1000 transactions|                          |
|    |Next 90M transaction $0.20 per 1000 transactions|                         |  |    |Above 100M transactions $0.05 per 1000 transactions|                       |
|    |Above 100M transactions $0.05 per 1000 transactions|                       |

### Language

The language application package aims to add natural language processing tools to developers in the form of API and SDK. 

#### Immersive Reader

Immersive reader is a preview only service to add AI text to speech integration for accessibility services [@cognitve-reader-overview-sp20-516-243]. In preview, this feature is free and pricing out of preview is unavailable. The SDK packs for this projects are limited to Swift, node.js, and ASP.NET Core. The main features of immersive reader are text to speech, focused reading windows, visual reading cues, and syllable-word breakdown [@cognitve-reader-details-sp20-516-243]. 

#### Language Understanding

Language Understanding is a pretrained natural language processor [@cognitve-language-overview-sp20-516-243]. It is available through SDK using C#, Python, and JavaScript. It is additionally available using REST in all REST compatible languages. Free versions of language understanding can process typed language; whereas, the paid version can process both typed and spoken language. Language understanding can be applied to bot services or IoT control. 

|Instance|Transactions per Secong (TPS)|Features|Price [@cognitve-language-pricing-sp20-516-243]|
|---     |---                          |---     |---|
|Free Web/Container|	5 TPS |	Text Requests|10,000 transactions free per month|
|Standard|50 TPS|Text Requests|$1.50 per 1000 transactions|
|||Speech Requests|$5.50 per 1000 transactions|

#### QnA Maker

QnA Maker uses Knowledge base databases to create a chat bot [@cognitve-qna-overview-sp20-516-243]. It can be customized to different levels of formality. It allows for additional processes to be added over time. It supports C#, Python, and JavaScript. For knowledge base integreation it supports cURL and Postman [@cognitve-qna-curl-sp20-516-243].

|Instance|Transactions per Secong (TPS)|Limitations |Price [@cognitve-qna-pricing-sp20-516-243]|
|---     |---                          |---     |---|
|Free Web/Container|	3 TPS |	Up to 1MB each document|
|                 |         |Up to 100 transactions per minute|
|                 |         |Up to 50,000 transactions per month|
|                 |         |3 managed documents free per month|
||||
|Standard|3 TPS|Up to 100 transactions per minute|$10 for unlimited managed documents|

#### Text Analytics

Text analytics aims to provide broad range text analytic service in SDK packaging. The key features are sentiment analysis, key phrases extraction, named entities extraction and language determination. There is SDK available for C#, Python, Node.js, Go, and Ruby. It provides easy integration to Power BI and Flask. [@cognitve-analytics-overview-sp20-516-243]

|Instance|Features|Price [@cognitve-analytics-price-sp20-516-243]|
|---|---|---|
|Free    |Sentiment Analysis      |N/A|
|        |Key Phrase Extraction   ||
|        |Language Detection      ||
|        |Named Entity Recognition||
|        |                        ||
|Standard|Sentiment Analysis|0-500,000 text records: $2 per 1,000 text records|
|        |Key Phrase Extraction|0.5M-2.5M text records: $1 per 1,000 text records|
|        |Language Detection| 2.5M-10.0M text records: $0.50 per 1,000 text records|
|        |Named Entity Recognition|10M+ text record: $0.25 per 1,000 text records |

#### Translator Text

The translator text API provides neural translator services for developer integration. It is available in C# and REST API. Azure marketing tools indicate that it is useful for increasing research text data, detecting input language, bilingual dictionary tools, on device translation, and custom trained translation. [@cognitve-translate-overview-sp20-516-243]

|Instance|Features|Price [@cognitve-translate-price-sp20-516-243]|
|---|---|---|
|Free|Standard Translation|2M Characters Free|
|    |-Text Translation||
|    |-Language Detection||
|    |-Bilingual Dictionary||
|    |-Transliteration||
|    |Custom Translation||
|    |-Training||
||||
|S1  |Standard Translation|Standard|
|    |-Text Translation|- $ 10 per million characters|
|    |-Language Detection||
|    |-Bilingual Dictionary|Custom|
|    |-Transliteration|- $ 40 per million chars of custom translation|
|    |Custom Translation|- $ 10 per million source + target chars of training data (max. $ 300/training)|

### Speech

Speech packages adds additional natural language processing tools to developers for spoken language. Azure provides API access through REST API as well as SDK in C++, C#, Java, JavaScript, Objective-C, and Python. 

#### Speech to Text

The speech to text tool uses neural network speech recognition algorthms to convert audiofiles to plaintext [@cognitve-stt-overview-sp20-516-243]. Its applications include accesibility for the deaf and hard of hearing and domain specific vocabulary transcription.

|Instance|Features|Price [@cognitve-speech-price-sp20-516-243]|
|---|---|---|
|Free|Standard|5 audio hours free per month|
|   |Custom|5 audio hours free per month. 1 model free per month|
|   |      |                                                    |
|Standard|Standard|$1 per audio hour|
|        |Custom|$1.40 per audio hour. Endpoint hosting: $0.0538 per model per hour|


#### Text to Speech

Azure Text to Speech is a neural network text to speech tool that is meant to provide life-like voice synthesis to applications. [@cognitve-tts-overview-sp20-516-243] Azure provides both access to pretrained models and the abiltiy to create unique voice models for specific applications.This can be used in place of immersive reader for accessibility features meant for blind individuals. 


|Instance|Features|Price [@cognitve-speech-price-sp20-516-243]|
|---|---|---|
|Free|Standard|5M characters free per month|
|   |Neural|0.5M characters free per month|
|   |Custom|5M characters free per month. Endpoint hosting: 1 model free per month|
|   |     |                              |
|Standard|Standard|$4 per 1M characters|
|   |Neural|$16 per 1M characters|
|   |Custom| $6 per 1M characters. Endpoint hosting: $0.0537 per model per hour |
|   |Custom Neural|Real-time synthesis: $24 per 1M characters. Endpoint hosting: $4.04 per model per hour. Long audio creation: $100 per 1M characters|

#### Speech Translation

Speech translation provides real time speech translation tools to applications. [@cognitve-transpeech-overview-sp20-516-243] Unlike speech to text and text to speech, speech translation is only cloud-based and will not operate on edge devices. 

|Instance|Price [@cognitve-speech-price-sp20-516-243]|
|---|---|
|Free|5 audio hours free per month|
|Standard|$2.50 per audio hour|

#### Speaker Recognition

Speaker recognition is a preview only tool available to developers. [@cognitve-speaker-overview-sp20-516-243] It is in early preview so the SDK's available for the other speech services are not ready currently. It is accessible through REST API. The service detects the speaker of an audio clip and names the entity, given that the entity has been captured previously. This can be used for multispeaker transcription services. As a preview, it is currently a free service.

### Vision

Azure Vision is an umbrella brand for the products using computer vision and image recogniton software. It includes the services Computer Vision, Custom Vision, Face, Form Recognizer, and Ink Recognizer.

#### Computer Vision

Computer vision is a pretrained computer vision model that can detect more than 10,000 ibjects. [@cognitve-comvis-overview-sp20-516-243] It can be trun in the cloud or in edge containers. Azure claims this service can be applied to robotic process automation, digital asset management, or to accesibillity features for the blind. The pricing strategy for computer vision is based on the object being detected. However, Azure provides 20 free transactions per minute. The full pricing detail can be found [here.](<https://azure.microsoft.com/en-us/pricing/details/cognitive-services/computer-vision/>) There is SDK available in .NET, Python, Java, Node.js, and Go.

#### Custom Vision

Custom vision allows fevelopers to custom train a computer vision model.[@cognitve-custvis-overview-sp20-516-243] It is optimized for small data inputs and large differences in objects. Azure warns that it is not optimal for quality assurance. The model can be exported for offline use. There is SDK available in .NET, Python, Java, Node.js, and Go. 

|Instance|Transactions per Second|Features|Price [@cognitve-custvis-overview-sp20-516-243]|
|---|---|---|---|
|Free|2 TPS|Upload, training, and prediction transactions. Up to 2 projects. Up to 1 hour training per month|5,000 training images free per project. 10,000 predictions per month|
|Standard|10 TPS|Upload and prediction transactions. Up to 100 projects|$2 per 1,000 transactions|
|        |      |Training|$20 per compute hour|
|        |      |Image Storage|$0.70 per 1000 images|

#### Face

The Face API is a facial detection and analysis software. [@cognitve-face-overview-sp20-516-243] It identifies the face and extracts features such as head pose, gender, age, emotion, facial hair, and eye wear detection. It can be used to verify identity and find similar faces or identical faces.  There is SDK available in .NET, Python, Java, Node.js, and Go.

|Instance|Tranactions per Minute|Price [@cognitve-face-price-sp20-516-243]|
|---|---|---|
|Free|20 TPM|30,000 transactions free per month|
|    |      |                                   |
|Standard|600 TPS|0-1M transactions - $1 per 1,000 transactions|
|       |       |1M-5M transactions - $0.80 per 1,000 transactions|
|       |       |5M-100M transactions - $0.60 per 1,000 transactions|
|       |       |100M+ transactions - $0.40 per 1,000 transactions |
|Face Storage|  |$0.01 per 1,000 faces per month|

#### Form Recognizer

Form recognizer takes images or PDFs and autopopulates their contents into custom or prebuilt forms.[@cognitve-form-overview-sp20-516-243] This may include pictures receipts, invoices, bills, or legal forms. The Form Recognizer can use supervised or unsupervised learning to populate the custom forms. It is only available using REST API or .NET SDK. 

|Instance|Document Type|Price [@cognitve-form-price-sp20-516-243]|
|---|---|---|
|Free| |0-500 pages Free per Month|
|Standard|Custom|$25 per 1000 pages|
|         |Pre-Built|$5 per 1000 pages|

#### Ink Recognizer

Ink Recognizer is a handwritting recognition software. [@cognitve-ink-overview-sp20-516-243] It can be used with pen and paper interactions or digital handwriting. Azure suggests applying this service to notetaking, form-filling, content search, and documentation annotation. 

|Instance|Price [@cognitve-ink-price-sp20-516-243]|
|---|---|
|Free|2000 transactions free per month|
|Standard| 	$2 per 1,000 transactions|

## Example

One of the requirements for the chapter submission for this class is to present objective documentation of the service and not to advertise for the company. This can be done using Azure's Text Analytics service [@cognitve-text-code-sp20-516-243]. 

1) The first step is to create an account on Azure. 

2) Direct your browser to <https://azure.microsoft.com/en-us/> and click on start free.

3) After signing up for a free account, go to <https://portal.azure.com/>. 

4) Open the side bar and click "Create a new resource." This should bring up a menu of available resources. 

5) You will then click on "AI + Machine Learning." If "Text Analytics" is on the featured page, select that and skip to the next step; otherwise, direct to "See All." You will see a heading "Cognitive Services." Select "See More" under this heading. You will then see all available cognitive services resources. Select "Text Analytics."

6) Select "Create" and make a name, select your desired server location and pricing tier (this will allow you to select the free pricing tier). You will then select a resource group if you have made one already or create a new one. Creating a new resource group is simply giving the virtual machine a name. Once you have finished, select "Create."

7) Direct to <https://portal.azure.com/> and select your newly created Texts Analytics page. It will have the name you made as well as type listed as "Cognitive Services." 

8) Click "Quick Start" on the right hand menu. Then you will see your key1 and endpoint key. You will need this for your enviroment variables. 

9) Instal Azure text analytics using the command

```
!pip install azure-ai-textanalytics
```

10) Open the Python editor of your choice and set the enviroment variables  with the following syntax


```
key = "ENTER YOUR KEY1 VARIABLE HERE"
endpoint = "ENTER ENDPOINT VARIABLE HERE
```

11) You will then need to authenticate your usage using the following code. 

```
from azure.ai.textanalytics import TextAnalyticsClient, TextAnalyticsApiKeyCredential
def authenticate_client():
    ta_credential = TextAnalyticsApiKeyCredential(key)
    text_analytics_client = TextAnalyticsClient(
            endpoint=endpoint, credential=ta_credential)
    return text_analytics_client

client = authenticate_client()
```
12) You then have the ability to run the text analytics of your choice. As mentioned in the text analytics section,features like sentiment anlaysis, key feature extraction, and entity tagging are all available through the texts analytics API. Sentiment analysis can be used to determine whether your chapter demonstrates the required objectivity.The sentiment analysis can be coded as a fucntion.

```
def sentiment_analysis_example(client, docu):
    # Turns function into a format that fucntion can use.
    document = [docu]
    docu = docu.replace('\n', ' ')
    sentences=[docu.split('. ')]
    response = client.analyze_sentiment(inputs=document)[0]
    # Overall sentiment.
    print("Document Sentiment: {}".format(response.sentiment))
    print("Overall scores: positive={0:.3f}; neutral={1:.3f}; negative={2:.3f} \n".format(
        response.sentiment_scores.positive,
        response.sentiment_scores.neutral,
        response.sentiment_scores.negative,
    ))
    for idx, sentence in enumerate(response.sentences):
        # If the positive sentiment score is above .5, returns the sentence and the sentiment breakdown. 
        if sentence.sentiment_scores.positive > .5:
          # This requires that all sentences have a period followed by either a space or a newline. 
          print(sentences[0][idx])
          print("[Offset: {}, Length: {}]".format(sentence.offset, sentence.length))
          print("Sentence {} sentiment: {}".format(idx+1, sentence.sentiment))
          print("Sentence score:\nPositive={0:.3f}\nNeutral={1:.3f}\nNegative={2:.3f}\n".format(
              sentence.sentiment_scores.positive,
              sentence.sentiment_scores.neutral,
              sentence.sentiment_scores.negative,
        ))
```

13) Now call your document. You may analyze up to 1520 characters at a time. 

```
docu = """ 
INSERT CHAPTER HERE
 """

sentiment_analysis_example(client, docu)

```
13) Now you may change your chapter according to the feedback from the Azure sentiment analysis. 
