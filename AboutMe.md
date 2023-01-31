# Pravallika Mummadi

Interesting facts about me are rare because i am boring person. The more boring person i am , my life is less dramatic.I love to travel a lot and explore adventurous things ,also very fond of cooking pizza and burger.

 ![Image](aboutPIC.JPG)

 ***************
 Below is the table that recommends countries to the travellers to visit on their vacation

 |Name of the Country|The reason for recommending|Days to spend|
| :--- | :---: | ---: |
 | India | Visit the Ancient temples and cuisines from different states | 30 |
 | Italy | To watch Eiffel tower and original Pizza | 30|
 | Switzerland | Feel the nature | 30 |
 | Australia | Good for Tourism | 30 |

 *************
 > The funniest quote i came across is :

 >**"Screenshots destroy the relationships"** -- *Pravallika Mummadi*

 >**"Have a cup of coffee when you are happy,bored,sad"** -- *Pravallika Mummadi*

 *************
  Link for the article <https://docs.aws.amazon.com/marketplace/latest/userguide/saas-code-examples.html> 
 ># ResolveCustomer code with x-amzn-marketplace-token token for a CustomerIdentifier, ProductCode, and CustomerAWSAccountId. 

 ```
 //Import AWS Python SDK and urllib.parse 

import boto3

import urllib.parse as urlparse 

//Resolving Customer Registration Token

formFields = urlparse.parse_qs(postBody)

regToken = formFields['x-amzn-marketplace-token']

//If regToken present in POST request, exchange for customerID

if (regToken):

    marketplaceClient = boto3.client('meteringmarketplace')

    customerData = marketplaceClient.resolve_customer(regToken)

    productCode = customerData['ProductCode']

    customerID = customerData['CustomerIdentifier']

    customerAWSAccountId = customerData['CustomerAWSAccountId']

    # TODO: Store customer information 
    # TODO: Validate no other accounts share the same customerID
 ```


Lets go to the code snippet <https://docs.aws.amazon.com/marketplace/latest/userguide/saas-code-examples.html> 



