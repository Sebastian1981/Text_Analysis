# Extracting insights from text using the Azure language service

The language service was used to:
- identify language
- extract keywords
- sentiment analysis
- entity recognition
- extract related entities

## Language identification
The language recognition API evaluates text input and returns language IDs for each submitted document with a score that indicates the reliability of the analysis. The language service recognizes up to 120 languages.

## Extract keywords
Key phrase extraction is the process of parsing the text of a document or documents and then identifying the most important statements in the context of the document or documents.

## Sentiment analysis
Sentiment analysis is used to assess how positive or negative a text document is, which can be useful in various workloads, e.g. rating a movie, book, or product by quantifying sentiment based on reviews or prioritize customer service responses to correspondence received via email or social media messages.

## Entity recognition
Named entity recognition identifies entities that are mentioned in the text. Entities are grouped into categories and subcategories, e.g. person, location, datetime, organization, address, e-mail or URL
## Extract related entities
In some cases, the same name can be applicable to multiple entities. An instance of the word "Venus" can refer on the planet or the Greek goddess.

Entity linking can be used to disambiguate entities with the same name by referencing an article in a knowledge base. Wikipedia provides the knowledge base for the text analysis service. Specific article links are determined based on the entity context within the text.

For example, "I saw Venus shining in the sky" links to https://en.wikipedia.org/wiki/Venus, while "Venus, goddess of beauty" links to https://en.wikipedia.org/wiki/ Venus_(mythology) is linked.

## Get the script running
- create the required azure ressources
- set up a python 3.8 environment 
- open terminal and run: $pip install azure-ai-textanalytics==5.1.0
- create .env file and insert the required COG_SERVICE_ENDPOINT and COG_SERVICE_KEY
 