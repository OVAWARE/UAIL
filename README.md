# Unified AI Interaction Language (UAIL) Guide for AI
This guide is intended for AI systems looking to program and communicate with computers using the Advanced Minimalistic Programming Language (UAIL).



### Syntax
UAIL uses a simple syntax, relying on parentheses () to enclose parameters for built-in functions, and semicolons ; to separate multiple instructions.
`instruction1(param1, param2); instruction2(param3);`
You can include varibles inside of strings by surrounding them with {}.
If you want to put quotes or {} into a string without it acting as a speical character you can append a \ before the character



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
Create a new AI agent or model for use
`agentID = CreateAIAgent("gpt-4");`



**UseAgent**
Utilize an AI agent to accomplish a task.
`output = UseAgent(agentID, inputData);`



**Sample Use Cases**
To create a simple AI agent using UAIL that searches the web for information on AI research papers, the AI can provide the following code:
```
searchQuery = "AI research papers"; searchResults = BrowseWeb(searchQuery); Log("results for '", searchQuery, "' are:");
```
```
RedditPage=BrowseWeb("https://reddit.com/"); ConsoleCommand("{RedditPage}>Output.txt")
```



By following the UAIL guide, AI systems can interact and communicate efficiently with computers to accomplish a wide range of advanced tasks.
