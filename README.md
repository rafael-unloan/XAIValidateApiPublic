## Welcome to Xapii by Tiimely

Use our Xapii API documentation to begin your **pursuit of seamless**. At Tiimely, we provide some of Australia's most prominent lenders and brands with highly configurable solutions that businesses can use throughout their lending offerings. 

Market leaders in home lending, consumer lending, credit cards, auto finance, and hardship utilise Xapii APIs to complement, not replace, their existing tech stack to optimise customer outcomes, create engaging journeys, and meet compliance obligations. 
 
With Xapii APIs, you can:
  - Convert - reduce time and cost to 'yes' with tools that improve conversion
  - Decide - Automated real-time lending decisioning configured to your product and policy requirements
  - Fulfil - create a faster, more compliant path to loan completion
  - Inform - leverage Tiimely's data capabilities and insights to mitigate risks and identify business growth opportunities

Ready to start your pursuit of seamless?

[Contact us](mailto:contact@tiimley.com) to discuss which product is right for you and to gain access to our sandbox.
 
### Xapii by Tiimely supports a range of data sources, including:
  - Popular data aggregators (illion or Yodlee)
  - Connect your own data
  - Consumer Data Right (CDR)
  - Comprehensive Credit Report (CCR) data - coming soon!
  - Digitised documents (OCR) - coming soon!

The following table provides information on the data sources that are supported and the essential details to include your requests. By default, you can use two data sources — your selected data aggregator and the option 'connect your own data'.
    
  |**Data Source**|**Data Provider Name**|**Date Provider Reference**|**Details**|
  |---|---|---|---|
  |illion ODS BrokerFlow|`ODS`|A list of your BrokerFlow `DocumentIds`.|You can provide multiple `DocumentIds` for each applicant.|
  |illion ODS MultiBank|`MB`|None|We will provide a unique URL for each applicant. When used by your customers, their accounts will link and their data will automatically sync to the corresponding application in Xapii.|
  |Yodlee v1.1|`YOD11`|A list of your Yodlee customer identifiers.|There is a one-to-one linking of the applicant to the Yodlee customer identifier.|
  |Yodlee v1.1 (CDR "outsource service provider")|`YOD11`|A list of your Yodlee customer identifiers.|There is a one-to-one linking of the applicant to the Yodlee customer identifier.|
  |Connect your own data|`EXT`|None|When using external API data (`EXT`) you'll be required to upload your data to the application. Check out `/financialvalidation/provideaccounts` for more information.|
          
## Getting Started  
  The Xapii by Tiimely API provides a way to seamlessly integrate assessment of financial poistion into your workflow. The table below provides a summary of endpoints, which allow you to get "data in" and then "data out". You can use the [Xapii by Tiimely user interface](https://app.tiimely.com) at any time to interact with your data and the automated assessment of financial position.
  
You'll need the following to start developing:
  - sign-up for Xapii by Tiimely. [Contact us](mailto:contact@tiimley.com) to discuss the right product and access to our `sandbox`
  - your client credentials for the Xapii by Tiimely user interface and API. These will provided to you by Xapii by Tiimely, and must be stored securely
  - you're then ready to start developing against our test environment using the endpoints below. 
  

## Data Model  
  
When you interact with the Xapii by Tiimely user interface and APIs you'll notice there's a clear structure to the data. We've designed the Xapii by Tiimely data model to be optimised for automating assessment of financial position. The data hierarchy is:
  - **application**: this is the structure that holds all other elements and represents a point-in-time product application from your customer
  - **applicants**: an application can have one or more applicants (currently limited to two). Applicants can belong to multiple applications, e.g. a customer applying for a credit card and a home loan would exist in two applications
  - **households**: your applicants belong to households. For convenience we will assign applicants to a single, default household at the start of application
  - **accounts**: applicants own accounts, which can be held individually or jointly with the other  applicant on the application
  - **transactions**: these are the credits and debits against each account. Transactions are enriched with attributes such as categories, high risk flags and expense management. 
  - **documents**: each application and applicant can have a document linked, each with a defined type and format.
  
## References

Here are a few resources to help you on your way:
  - **User guide**: you can access this through the Xapii by Tiimely application. Simply login and navigate to your name in the top right.
  - **SDKs**: coming soon
  - **Postman 'Collection'**: download this collection to help you interact with the Xapii by Tiimely APIs using Postman (coming soon).
