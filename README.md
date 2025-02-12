# Job Search Assistant

A POC project using the RAG technique (Retrieval-Augmented Generation) paired with OpenAI's models to 
implement a [SurelyWork.com](https://surelywork.com/) Job Search Assistant. The Job Search Assistant is a conversational way
to help job seekers find relevant job listings on Surely Work.

The RAG is implemented using vector database similarity search to enrich the LLM prompt with relevant job listing data. The LLM then does the magic of replying back with a seamless natural language response.

## Running

To start copy the .env.template to .env and add your OpenAI API key.


From there just run the following commands:
`npm install`
`npm run start`

If you'd like you can update the actual input text in the `src/index.ts` file.

## Blog Post

Check out [the post](https://www.ericventor.com/posts/leveraging-vector-stores-for-LLM-prompts) on my blog more information about enriching prompts
using vector databases!

## Example

Here's an example of an interaction with the Job Search Assistant, where a fashion designer is seeking a job:

> Input: "I'm a fashion designer based in Los Angeles."
> 
> Output:
> "That's great to hear! As a fashion designer based in Los Angeles, you might be interested in a couple of job listings we have on SurelyWork.com:
> 
> LA Fashion Week: Designer Casting Call by Asal Etemadi: They are looking for independent designers to showcase their work on their runway during LA Fashion Week. > It's a great opportunity to have your designs come to life alongside mesmerizing music performances. The deadline to submit your designs is September 23rd. You can > find more information and apply here.
> 
> Casting Call for Jewelry Brand by Jacqueline Kulla: They are specifically looking to cast redheads for a shoot for their jewelry brand. If you have red hair, this > could be a great opportunity for you. The details and application can be found here.
> 
> Feel free to check out these listings and apply if they align with your interests and skills. Let me know if there's anything else I can assist you with!"

As demonstrated, the LLM successfully utilizes data from relevant job listings in its response and even includes links to them.# Ai-job-search-assistant
