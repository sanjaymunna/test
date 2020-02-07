# api-souring-product

Module used for convert feed data of Products into a WCM. 

## Prerequisites

 - OpenJDK 11
 - Maven 3.6.0+
 - Kafka

## Configuration

The configuration can be passed via environment variables as follows:

###  Configuration via environment variable:

Please set the following environment variable:
#### 1.              On Linux
	export feedPath = "/home/feed"



#### 2.            	Windows
	set feedPath = "C:\\feed\\"





#### Request Payload for Product of Ingredient, Simple Item, Option Set, Option Set Item, Customized Item, Offer Group, and Offer on Offer Feed processing:-


#### API endpoint : 
	http://<IPAddress>:<PORT_NO>/commerce/products

#### Method Type :	POST

#### Body :
  

#### 1.   Ingredient
        {
		"itemClassification":"Ingredient",
		"fileNames":["Ingredients ( IC).csv"]
	}
#### 2. Simple Item
	{
		"itemClassification":"Simple Item",
		"fileNames":["Simple Items (FPS).csv"]
	}
#### 3. Option Set
	{
		"itemClassification":"Option Set",
		"fileNames":["Option Set - Header.csv"]
	}
#### 4. Option Set Item
	{
		"itemClassification":"Option Set Item",
		"fileNames":["Option Set - Items (1).csv"]
	}
#### 5. Customized Item
	{
		"itemClassification":"Customized Item",
		"fileNames":["Customized Items ( FPC) - Header.csv", "Customized Items ( FPC) - Item.csv"]
	}
#### 6. Offer Group
	{
		"itemClassification":"Offer Group",
		"fileNames":["Offer Grouping (OG) - Header.csv", "Offer Grouping (OG) - Item.csv"]
	}
#### 7. Offer on Offer
	{
		"itemClassification":"Offer on Offer",
		"fileNames":["Offer on Offer (OO) - Header.csv", "Offer on Offer (OO) - Item (1).csv"]
	}

