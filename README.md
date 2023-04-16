# Unified AI Interaction Language (UAIL) Guide for AI
This guide is intended for AI systems looking to program and communicate with computers using the Advanced Minimalistic Programming Language (UAIL).



### Syntax
UAIL uses a simple syntax, relying on parentheses () to enclose parameters for built-in functions, and semicolons ; to separate multiple instructions.
`instruction1(param1, param2); instruction2(param3);`
Variables can be included inside strings by surrounding them with curly braces {}. If you want to put quotes or {} into a string without it acting as a special character, you can append a \ before the character.



### Variables
Variables don't require any type declaration, as their types are automatically assigned based on their initial values.
```
x = 42; message = "Hello, AI!";
```



### Built-in Functions
UAIL provides a set of advanced built-in functions to interact with computers, perform essential tasks, and utilize AI capabilities.



**ConsoleCommand**
Execute a command in the terminal or command prompt.
`output = ConsoleCommand("ls");`



**Log**
Display a message or a value.
`Log("AI is working!");`



**EvalPython**
Evaluate a Python expression or code and return the result. To perform more complex tasks or calculations, pass in the necessary Python code as a string.
`result = EvalPython("5 + 10");`



**BrowseWeb**
Search for specific content on the web, and return relevant results as a list of URLs or text.
`searchResults = BrowseWeb("AI research papers");`



**CreateAIAgent**
Create a new OpenAI agent to use. AgentID can be used to control the agent
`agentID = CreateAIAgent("gpt-4");`



**UseAgent**
Utilize an AI agent to accomplish a task.
`output = UseAgent(agentID, inputData);`



**DeleteAgent**
Deletes a Agent by AgentID when its task is done.
`DeleteAgent(agentID);`



**Sample Use Cases**
To create a simple AI agent using UAIL that searches the web for information on AI research papers and prints the result
```
searchQuery = "AI research papers"; searchResults = BrowseWeb(searchQuery); Log("Results for {searchQuery} are {searchResults}");
```
Read reddits homepage and store the result in Output.txt
```
RedditPage=BrowseWeb("https://reddit.com/"); ConsoleCommand("{RedditPage}>Output.txt")
```
Get the current date and time and display a personalized message
```
time = EvalPython("from datetime import datetime; datetime.now().strftime('%Y-%m-%d %H:%M:%S')"); username = "JohnDoe"; Log("Hello, {username}! The current date and time is: {time}");
```
Query an AI agent to write a brief introduction about AI
```
inputData = "Briefly introduce Artificial Intelligence."; agentID = CreateAIAgent("gpt-4"); intro = UseAgent(agentID, inputData); DeleteAgent(agentID); Log("AI Introduction: {intro}");
```



By following the UAIL guide, AI systems can interact and communicate efficiently with computers to accomplish a wide range of advanced tasks.
