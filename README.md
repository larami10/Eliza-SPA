# Eliza Single Page Application (SPA)

A simple attempt to recreate Eliza as a Single Page Application with the following features:

1. Eliza's dictionary of responses comes from dictionary.json
2. Eliza will ask the user for their name.
   1. If user sends a blank input, Eliza will reply with a random response and ask the user for their name again.
   2. If user enters a name, Eliza will "remember" the name and continue to use that name in the conversation that follows.
3. After a name is entered, Eliza will:
   1. display the entire conversation on the single page
   2. begin asking random questions
   3. parse the user's input
   4. throw a random message from a pool of appropriate responses if a word matches a key property in Eliza's dictionary
   5. throw a random message from a pool of "noInput" if a word does not match a key property in Eliza's dictionary
4. If the user doesn't respond after 20 seconds, Eliza will throw an alert with a random message to get the user's attention.
5. Eliza will save conversations (state) per name in local storage. If a user restarts the program and enters a name that already had a conversation with Eliza, Eliza will "restore" that user's conversation.
6. Eliza understands special commands:
   1. Entering "/clear" will clear the state of the application for that name (delete them from local storage) and return to the starting form.
   2. Entering "/search key" will search the conversation for the most recent user input containing key, and copies that entire previous input into the one-line user input area. (This feature is better tested with full sentence inputs)

> **_NOTE:_** Eliza was Alexa before Alexa. For more information, please check out the following links:

[Eliza, the Rogerian Therapist](http://psych.fullerton.edu/mbirnbaum/psych101/Eliza.htm)
[Eliza on Wikipedia](https://en.wikipedia.org/wiki/ELIZA)

## How to use the Project

You can clone the repository and cd into the project folder:

```
cd Eliza-SPA
```

From the Eliza-SPA folder, open the Eliza-SPA.html file in a browser and begin talking to Eliza.
