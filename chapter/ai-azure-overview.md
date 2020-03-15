#  AI Services on Azure

* sp20-516-243 David Drummond

Azure is the Microsoft cloud computing platform. Azure operates through a multiplicity of data centers in order the the information processing to occur in closer physical proximity to end users. Azure initially lauched in 2010 and the public deployment of its Machine learning arm occured in 2014. The following overview of the AI services on Azure encompasses only the applications that Azure has listed as "AI." 

Azure AI is a set of AI services built on Microsoft’s research and innovation in vision, speech, language processing, and custom machine learning [sp20-516-238-azure-bot-service-overview]. 

**Azure AI helps organizations:**

* Develop machine learning models that can help with scenarios such as demand forecasting, recommendations, or fraud detection using Azure Machine Learning.
* Incorporate vision, speech, and language understanding capabilities into AI applications and bots, with Azure Cognitive Services and Azure Bot Service.
* Build knowledge-mining solutions to make better use of untapped information in their content and documents using Azure Search.

## Azure Cognitive Services

Cognitive services is a service from Azure that is intended for devolpers with little ML understanding of experience [@azure-ai-sp20-516-243] . It provides out of the box tools including :

<div class="smalltable">
  
| Service | Description |
|---------|-------------|
| [Anomoly Detector](<https://azure.microsoft.com/en-us/services/cognitive-services/anomaly-detector/>) | Allows decision makers to easily detect sudden changes in data patterns.|
| [Content Moderator](<https://azure.microsoft.com/en-us/services/cognitive-services/content-moderator/>) | Detectss potentially illicit or offensive content in user content. |
| [Personalizer](<https://azure.microsoft.com/en-us/services/cognitive-services/personalizer/>) | Uses reinforcement learning to tailor end-user expereince. |
| [Immersive Reader](<https://azure.microsoft.com/en-us/services/cognitive-services/immersive-reader/>) | A reading assist tool for those with lower reading ability levels. |
| [Language Understanding](<https://azure.microsoft.com/en-us/services/cognitive-services/language-understanding-intelligent-service/>) | A natural language processor for edge computing and IoT. |
| [QnA Maker](<https://azure.microsoft.com/en-us/services/cognitive-services/qna-maker/>) | A conversational bot designed as an overlay for knowledge libraries. |
| [Text Analytics](<https://azure.microsoft.com/en-us/services/cognitive-services/text-analytics/>) | A language processor to extract sentiment and key phrases from text inputs. |
| [Translator Text](<https://azure.microsoft.com/en-us/services/cognitive-services/translator-text-api/>) | Translation algorithm for 60 languages. |
| [Speech to Text](<https://azure.microsoft.com/en-us/services/cognitive-services/speech-to-text/>) | Enables searchable and readable transcription services. |
| [Text to Speech](<https://azure.microsoft.com/en-us/services/cognitive-services/text-to-speech/>) | Contains prebuilt neural Text to Speech engines as well as the ability to make personalized voice models. |
| [Speech Translation](<https://azure.microsoft.com/en-us/services/cognitive-services/speech-translation/>) | Gives real-time translation abilities to end users. |
| [Speaker Recognition](<https://azure.microsoft.com/en-us/services/cognitive-services/speaker-recognition/>) | Enables applications to recognize the voices of speakers in audio. |
| [Computer Vision](<https://azure.microsoft.com/en-us/services/cognitive-services/computer-vision/>) | Enables image recognition. |
| [Custom Vision](<https://azure.microsoft.com/en-us/services/cognitive-services/custom-vision-service/>) | Domain specific computer vision engine. |
| [Face](<https://azure.microsoft.com/en-us/services/cognitive-services/face/>) | Tool to compare facial images. |
| [Form Recognizer](<https://azure.microsoft.com/en-us/services/cognitive-services/form-recognizer/>) | Extracts data from images of forms. |
| [Ink Recognizer](<https://azure.microsoft.com/en-us/services/cognitive-services/ink-recognizer/>) | Recognizes handwritting and converts it to text. |
| [Video Indexer](<https://azure.microsoft.com/en-us/services/media-services/video-indexer/>) | Metadata analysis of videos. |

## Azure Machine Learning

Azure Machine Learning can be used for any kind of machine learning, from classical ml to deep learning, supervised, and unsupervised learning. From writing Python or R code or zero-code/ low-code options such as the designer, Azure Machine Learning Workspace can help build, train, and track highly accurate machine learning and deep-learning models [sp20-516-238-azure-machine-learning].

Azure Machine Learning provides rich set of tools required by developers and data scientists, which includes:

*  The Azure Machine Learning designer (preview): drag-n-drop modules to build your experiments and then deploy pipelines.
* Jupyter notebooks: use our example notebooks or create your own notebooks to leverage our SDK for Python samples for your machine learning.
* R scripts or notebooks in which you use the SDK for R to write your own code, or use the R modules in the designer.
* Visual Studio Code extension
* Machine learning CLI
* Open-source frameworks such as PyTorch, TensorFlow, and scikit-learn and many more

![Open and Flexible Azure ML Platform [sp20-516-238-azure-ml-platform]](images/azure-ml-platform.png){#fig:azure-ml-platform-open&flexible}

### Machine Learning Lab

Azure's machine learning lab is a multifaceted machine learning container platform intended to give machine learning practitioners to create and deploy custom ML models. Azure focuses highly on MLOps- a play on DevOps for machine learning practitioners While machine learning focused containers are free on Azure, access to the Azure designed features of MLOps are corporate priced features and are inaccesible for student use [@azure-ml-sp20-516-243]. 

## Bot Services

Azure bot service provides the tools to create chat bots for enterprise solutions [@azure-bot-sp20-516-243]. The SDK allows integration with the cognitive services to allow intelligent chat services. It is availble for a mulitude of platforms including Facebook, kik, Microsoft Teams, Slack, and WhatsApp. 


</div>

