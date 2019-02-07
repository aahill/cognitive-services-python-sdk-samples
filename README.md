---
services: cognitive-services
platforms: python
author: lmazuel
---

# Cognitive Services Python SDK Samples

These samples will show you how to get up and running using the Python SDKs for several Azure Cognitive Services. They demonstrate some of the services' features, and how to interact with the data from them.

## Featured services

This project framework provides examples for the following services:

### Knowledge

| Cognitive Service                                                               | Python package                                                                                                       | Documentation                                                                        |
|---------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------|
| [QnA Maker](https://azure.microsoft.com/services/cognitive-services/qna-maker/) | [azure-cognitiveservices-knowledge-qnamaker](http://pypi.python.org/pypi/azure-cognitiveservices-knowledge-qnamaker) | [QnA Maker documentation]() |

### Language

| Cognitive Service                                                               | Python SDK package                                                                                                       | Documentation                                                                        |
|---------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------|
| [Bing Spell Check](https://azure.microsoft.com/services/cognitive-services/spell-check/) |[azure-cognitiveservices-language-spellcheck](http://pypi.python.org/pypi/azure-cognitiveservices-language-spellcheck) | [Bing Spell Check documentation](https://docs.microsoft.com/azure/cognitive-services/bing-spell-check/) |
| [Language Understanding(LUIS)](https://docs.microsoft.com/azure/cognitive-services/luis/) | [azure-cognitiveservices-language-luis](http://pypi.python.org/pypi/azure-cognitiveservices-language-luis) | [LUIS Documentation](https://docs.microsoft.com/azure/cognitive-services/bing-spell-check/) |
| [Text Analytics](https://azure.microsoft.com/services/cognitive-services/text-analytics/) | [azure-cognitiveservices-language-textanalytics](http://pypi.python.org/pypi/azure-cognitiveservices-language-textanalytics) | [Text Analytics Documentation](https://docs.microsoft.com/azure/cognitive-services/text-analytics/) |

### Search

| Cognitive Service                                                               | Python SDK package                                                                                                       | Documentation                                                                        |
|---------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------|
| [Bing Autosuggest](https://azure.microsoft.com/services/cognitive-services/spell-check/) |[azure-cognitiveservices-search-autosuggest](http://pypi.python.org/pypi/azure-cognitiveservices-search-autosuggest) | [Bing Autosuggest documentation](https://docs.microsoft.com/azure/cognitive-services/bing-autosuggest/) |
| [Bing Custom Search](https://azure.microsoft.com/services/cognitive-services/bing-custom-search/) | [azure-cognitiveservices-search-customsearch](http://pypi.python.org/pypi/azure-cognitiveservices-search-customsearch) | [Bing Custom Search Documentation](https://docs.microsoft.com/azure/cognitive-services/bing-custom-search/) |
| [Bing Custom Image Search](https://azure.microsoft.com/services/cognitive-services/bing-custom-search/) | [azure-cognitiveservices-search-customimagesearch](http://pypi.python.org/pypi/azure-cognitiveservices-search-customimagesearch) | [Bing Custom Image Search Documentation](https://docs.microsoft.com/azure/cognitive-services/bing-custom-search/) |
| [Bing Entity Search](https://azure.microsoft.com/services/cognitive-services/bing-entity-search-api/) | [azure-cognitiveservices-search-entitysearch](http://pypi.python.org/pypi/azure-cognitiveservices-search-entitysearch) | [Bing Entity Search Documentation](https://docs.microsoft.com/azure/cognitive-services/bing-entities-search/) |
| [Bing Image Search](https://azure.microsoft.com/services/cognitive-services/bing-image-search-api) | [azure-cognitiveservices-search-imagesearch](http://pypi.python.org/pypi/azure-cognitiveservices-search-imagesearch) | [Bing Image Search Documentation](https://docs.microsoft.com/azure/cognitive-services/bing-image-search/) |
| [Bing News Search](https://azure.microsoft.com/services/cognitive-services/bing-news-search-api) | [azure-cognitiveservices-search-newssearch](http://pypi.python.org/pypi/azure-cognitiveservices-search-newssearch) | [Bing News Search Documentation](https://docs.microsoft.com/azure/cognitive-services/bing-news-search/) |
| [Bing Video Search](https://azure.microsoft.com/services/cognitive-services/bing-video-search-api) | [azure-cognitiveservices-search-videosearch](http://pypi.python.org/pypi/azure-cognitiveservices-search-videosearch) | [Bing Video Search Documentation](https://docs.microsoft.com/azure/cognitive-services/bing-video-search/) |
| [Bing Visual Search](https://azure.microsoft.com/services/cognitive-services/bing-visual-search) | [azure-cognitiveservices-search-videosearch](http://pypi.python.org/pypi/azure-cognitiveservices-search-visualsearch) | [Bing Visual Search Documentation](https://docs.microsoft.com/azure/cognitive-services/bing-visual-search/) |
| [Bing Web Search](https://azure.microsoft.com/services/cognitive-services/bing-web-search-api) | [azure-cognitiveservices-search-websearch](http://pypi.python.org/pypi/azure-cognitiveservices-search-websearch) | [Bing Visual Search Documentation](https://docs.microsoft.com/azure/cognitive-services/bing-visual-search/) |


### Vision

| Cognitive Service                                                               | Python SDK package                                                                                                       | Documentation                                                                        |
|---------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------|
| [Computer Vision](https://azure.microsoft.com/services/cognitive-services/computer-vision/) |[azure-cognitiveservices-vision-computervision](http://pypi.python.org/pypi/azure-cognitiveservices-vision-computervision) | [Computer Vision documentation](https://azure.microsoft.com/services/cognitive-services/computer-vision/) |
| [Face](https://azure.microsoft.com/services/cognitive-services/face/) |[azure-cognitiveservices-vision-face](http://pypi.python.org/pypi/azure-cognitiveservices-vision-face) | [Face documentation](https://docs.microsoft.com/azure/cognitive-services/face/) |
| [Content Moderator](https://azure.microsoft.com/services/cognitive-services/content-moderator/) |[azure-cognitiveservices-vision-contentmoderator](http://pypi.python.org/pypi/azure-cognitiveservices-vision-contentmoderator)| [Content Moderator documentation](https://docs.microsoft.com/azure/cognitive-services/content-moderator/) |
| [Custom Vision](https://azure.microsoft.com/services/cognitive-services/face/) | [azure-cognitiveservices-vision-customvision](http://pypi.python.org/pypi/azure-cognitiveservices-vision-customvision)| [Custom Vision documentation](https://docs.microsoft.com/azure/cognitive-services/custom-vision/) |

We provide several meta-packages to help you install several packages at a time. Please note that meta-packages are only recommended for development purpose. It's recommended in production to always pin specific version of individual packages.

## Getting Started

### Prerequisites

* A Cognitive Services subscription key to authenticate your SDK calls. [Sign up here](https://azure.microsoft.com/services/cognitive-services/directory/) by navigating to the **Language** or **Search** services and acquiring an API key. You can get a trial key for **free** which will expire after 30 days or [create a Cognitive Services account](https://docs.microsoft.com/azure/cognitive-services/cognitive-services-apis-create-account#create-and-subscribe-to-an-azure-cognitive-services-resource) on the Azure portal through the *Use with an Azure subscription* button.

    > Subscription keys are usually per service. For example, the subscription key for Spell Check will not be the same than Custom Search. Read the previous *sign up* link or the Azure portal for details on subscription keys.

* [Python](https://www.python.org/downloads/)
    * This sample (and the SDK) is compatible with Python 2.7, 3.3, 3.4, 3.5 and 3.6.

It is generally recommended to use a Virtual Environment for Python development.

* Install and initialize the virtual environment with the "venv" module on Python 3 (you must install [virtualenv](https://pypi.python.org/pypi/virtualenv) for Python 2.7):

    ```
    python -m venv mytestenv # Might be "python3" or "py -3.6" depending on your Python installation
    cd mytestenv
    source bin/activate      # Linux shell (Bash, ZSH, etc.) only
    ./scripts/activate       # PowerShell only
    ./scripts/activate.bat   # Windows CMD only
    ```
    
    * For more information, see https://docs.python.org/3/tutorial/venv.html

### Get the repository and install the dependencies

1.  Clone the repository.

    ```
    git clone https://github.com/Azure-Samples/cognitive-services-python-sdk-samples.git
    ```

2.  Install the dependencies using pip.

    ```
    cd cognitive-services-python-sdk-samples
    pip install -r requirements.txt
    ```

### Create environment variables

For each service you want to use, create an environment variable on your machine that contains your subscription key.

Use the table below to find the environment variables you need to create.

### Knowledge
| Cognitive Service | Environment variable   |
|-------------------|------------------------|
| QnA Maker         | `QNA_SUBSCRIPTION_KEY` |

### Language
| Cognitive Service | Environment variable             | Notes                                                                                                                                                                                                                                                                                                    |
|-------------------|----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bing Spell Check  | `SPELLCHECK_SUBSCRIPTION_KEY`    |                                                                                                                                                                                                                                                                                                          |
| LUIS              | `LUIS_SUBSCRIPTION_KEY`          |                                                                                                                                                                                                                                                                                                          |
| Text Analytics    | `TEXTANALYTICS_SUBSCRIPTION_KEY` | Consider creating an environment variable named `TEXTANALYTICS_LOCATION` with your [Azure region](https://docs.microsoft.com/python/api/azure-cognitiveservices-language-textanalytics/azure.cognitiveservices.language.textanalytics.models.azureregions?view=azure-python) (westcentralus by default). |

### Search
| Cognitive Service        | Environment variable                 |
|--------------------------|--------------------------------------|
| Bing Autosuggest         | `AUTOSUGGEST_SUBSCRIPTION_KEY`       |
| Bing Custom Search       | `CUSTOMSEARCH_SUBSCRIPTION_KEY`      |
| Bing Custom Image Search | `CUSTOMIMAGESEARCH_SUBSCRIPTION_KEY` |
| Bing Entity Search       | `ENTITYSEARCH_SUBSCRIPTION_KEY`      |
| Bing Image Search        | `IMAGESEARCH_SUBSCRIPTION_KEY`       |
| Bing News Search         | `NEWSSEARCH_SUBSCRIPTION_KEY`        |
| Bing Video Search        | `VIDEOSEARCH_SUBSCRIPTION_KEY`       |
| Bing Visual Search       | `VISUALSEARCH_SUBSCRIPTION_KEY`      |
| Bing Web Search          | `WEBSEARCH_SUBSCRIPTION_KEY`         |

### Vision
| Cognitive Service        | Environment variable                | Notes                                                                                                                                                                                                                                                                                                       |
|--------------------------|-------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Computer Vision          | `COMPUTERVISION_SUBSCRIPTION_KEY`   | Consider creating an environment variable named `COMPUTERVISION_LOCATION` with your [Azure region](https://docs.microsoft.com/python/api/azure-cognitiveservices-language-textanalytics/azure.cognitiveservices.language.textanalytics.models.azureregions?view=azure-python) (westcentralus by default).   |
| Content Moderator        | `CONTENTMODERATOR_SUBSCRIPTION_KEY` | Consider creating an environment variable named `CONTENTMODERATOR_LOCATION` with your [Azure region](https://docs.microsoft.com/python/api/azure-cognitiveservices-language-textanalytics/azure.cognitiveservices.language.textanalytics.models.azureregions?view=azure-python) (westcentralus by default). |
| Custom Vision Training   | `CUSTOMVISION_TRAINING_KEY`         |                                                                                                                                                                                                                                                                                                             |
| Custom Vision Prediction | `CUSTOMVISION_PREDICTION_KEY`       |    

## Demo

A demo app is included to show how to use the project.

To run the complete demo, execute `python example.py`

To run each individual demo, point directly to the file. For example (i.e. not complete list):

2. `python samples/language/spellcheck_samples.py`
1. `python samples/search/entity_search_samples.py`
2. `python samples/search/video_search_samples.py`

To see the code of each example, simply look at the examples in the Samples folder. They are written to be isolated in scope so that you can see only what you're interested in.

## Resources

- [Azure SDK for Python](https://github.com/Azure/azure-sdk-for-python)
- [Azure SDK for Python reference](https://docs.microsoft.com/python/api/overview/azure/?view=azure-python)
- [Azure Cognitive Services Documentation](https://docs.microsoft.com/azure/cognitive-services/)

