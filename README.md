Set the following environment variables before running the application

1.            On Linux

export feedPath = "/home/feed"

2.            Windows

set feedPath = "C:\\feed"

-----------------------------------------------------------------------------
Request Payload for Product of Ingredient, Simple Item, Option Set, 
Option Set Item, Customized Item, Offer Group, and Offer on Offer Feed processing:-

URL:- http://<IP>:<PORT_NO>/commerce/products
Method Type:-POST
Body:-
1.   Ingredient
    {
		"itemClassification":"Ingredient",
		"fileNames":["Ingredients ( IC).csv"]
	}
b). Simple Item
	{
		"itemClassification":"Simple Item",
		"fileNames":["Simple Items (FPS).csv"]
	}
c). Option Set
	{
		"itemClassification":"Option Set",
		"fileNames":["Option Set - Header.csv"]
	}
d). Option Set Item
	{
		"itemClassification":"Option Set Item",
		"fileNames":["Option Set - Items (1).csv"]
	}
e). Customized Item
	{
		"itemClassification":"Customized Item",
		"fileNames":["Customized Items ( FPC) - Header.csv", "Customized Items ( FPC) - Item.csv"]
	}
f). Offer Group
	{
		"itemClassification":"Offer Group",
		"fileNames":["Offer Grouping (OG) - Header.csv", "Offer Grouping (OG) - Item.csv"]
	}
g). Offer on Offer
	{
		"itemClassification":"Offer on Offer",
		"fileNames":["Offer on Offer (OO) - Header.csv", "Offer on Offer (OO) - Item (1).csv"]
	}

