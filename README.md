## Building Customs Cleareance Agent with AutoGen.

Using llm to build a Customs Agent. 
Shipping companies process a large number of items that need customs clearance. For the items that require attention and need additional documents the sender and importer needs to be contacted.

This is repetative problem and can be solved with an Autonomous LLM based agent.

Following is an example of a workflow that the agent can follow.
- From a list of items identify the reason of holdup in clearing the shipment.
- If needed additional documentation, the agent generates appropriate email which contains the following information.
    1. If the item/s cannot be imported beacause of custom rules, please state those rules and politely mention the item cannot be imported.
    2. If the item/s can be imported but needs more info such as Price, bill of sale, country of origin or list of ingredients, please craft the email to list all the 
    required info from the customer.
    3. The email should include the customer care number.
- Send emails to customers.

## Running the jupyter notebooks

CLone the repo.

You will need the `OPENAI_API_KEY` saved in an `.env` file in the same directory.

And install the dependencies. 

## UI 

Need to figure out:

What would the UI for building such agents look like? [Agenthub.dev](https://www.agenthub.dev/), [Langflow.org](https://www.langflow.org/)?

How does the agent gets the data? csv, googlesheet, database access?

How does the agent send emails?

How do we make sure the Customs Rules and Regulations are the most recent and the LLM knows about it? Use Knowledge graph? RAG? 

Finetune the LLM on enterprise emails data?

Measure the margin of error.

Including a human in loop?

Implement image recognition for Item information.

