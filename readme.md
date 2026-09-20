Ai Agent Scaffold

How it works:
You put in your api key, and your browser directly queries gemini for steps on how to split your complicated task into minature tasks.
For each minature task, the previous input is fed back into gemini, with the addition of the minature task.
This is repeated until the task is complete.


Why it works:
LLM's like gemini usually have strict computational limits for each query and are worse at multistep problems.
By putting the workflow into an agentic loop, it bypasses these problems as each query only focuses on a single step, resulting in better answers.


Its using up all my tokens what do I do?:
You should switch to a worse model like gemini 3.5 flash-lite that uses less tokens to reduce usage. You can also directly ask the agent in the prompt to add less stuff.
We intend to add support for other ai providers in the future.


How to use it:
Simply paste your api key into the text box, put your prompt in and click run.
Wait for a few minutes for it to fully finish as gemini replies quite slowly.


Why would anyone use it compared to standard agentic platforms?:
This project is fully open source, which means users can rest easy knowing that their keys arent leaked.


What features does it have?:
It has built in model swapping so you can rest easy knowing that you are saving tokens on every step. The agentic loop also pastes only the last output back in
saving tokens and achieving almost equal performance.
