1. system prompt :
--prompt defines the system or it give instructions to a system 
--ex: act as social teacher,answer should be in bullet points etc
  so that the system now behave as social teacher,we can also give temp score( range is in btw 0 to 1 
   user prompt : 
-- prompt given by the user 
--ex: explain world war
   this is given by user

2. LLM-- model which trained on large data to give answer in less time where user ask question and the llm gives answer in same language ex:--gpt 4,gemini2.5 pro etc 
        Its not uptodated daily
        there are open source and close source
 api -- application programming interface
        its middleware btw the client and server , client request the api through payload and give it to the server and then api gives response to client 
inference -- it means run it can act as command 

workflow -- the flow of work like executing works/task one by one after completing the one work 

3. crawler through n8n
open n8n and go to canvas and click + there will be  AI select it after thst select  AI agent go back to canvas
after that at model which below the agent select the open ai chat model ,double click the model where you select the model that you want and come back to canvas
then we should select tool as of now select http request,  go to chatgpt or can done manually by looking at code which is in the firecrawl do the necessary paste url and add authorization ,content type and add body content 
save it and run 



4.role based prompting means the model that acts as what mentioned in prompt 
ex:act as doctor who has 15 years of experience in neuro 
   give output as bullet points
   tone should be confident 

5.
ollama run llama3-- run the model
ollama pull llama3-- pulls it , but it doesnt run

6.
from ollama import chat
from ollama import ChatResponse

response: ChatResponse = chat(model='gemma3', messages=[
  {
    'role': 'user',
    'content': 'Why is the sky blue?',
  },
])
print(response['message']['content'])
# or access fields directly from the response object
print(response.message.content)

7.
the purpose of a system role is to be specific and accurate of an output
without mentioning it , output answer will be in general 

8.

if we want want a real time output we cant get it through llm
so we use the tools like serpapi where we will connect ai agent with the serpapi tool to fetch real time information

ex: in chat we type latest news it goes through the flow and fetches information 

9.
act  as a helpful assistant who takes correct decisions and follow my commands 
the output should be precise and have enough information 
if doesnt know mention cannot help
say in confident


10.its not updated dailY
    SENSITIVE INFORMATION CAN BE  SAVED




