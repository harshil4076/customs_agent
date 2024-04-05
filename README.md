## Building Customs Cleareance Agent with AutoGen.

Using llm to build a Customs Agent. 
Shipping companies process a large number of items that need customs cleareance. For the items that require attention and need additional documents the sender and importer need to be contacted.

This repetative problem can be solved with an Autonomous LLM based agent.

Following is an example of a workflow that the agent can follow.
- From a list of items identify the reason of holdup in clearing the shipment.
- If needed documentation generate appropriate email which contains the following information.
    1. If the item/s cannot be imported beacause of custom rules, please state those rules and politely mention the item cannot be imported.
    2. If the item/s can be imported but needs more info such as Price, bill of sale, cuntry of origin or list of ingredients, please craft the email to list all the 
    required info from the customer.
    3. The email should include the customer care number so that the customer cn call.
- Send emails to customers.

