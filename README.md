<div align="center">
🚀 LM Studio Tools Integration
Supercharge your local AI with web-browsing capabilities!


![alt text](https://img.shields.io/badge/Model-Gemma_4-orange?style=for-the-badge)

![alt text](https://img.shields.io/badge/Browser-Brave-red?style=for-the-badge&logo=brave)
</div>
Welcome to the LM Studio Tools repository! This setup allows you to integrate functional tool-calling (like web searching) into your local LM Studio environment using the powerful Gemma 4 model.
📋 Prerequisites
Before diving in, make sure you have the following installed on your machine:
🦁 Brave Browser: Used as the secure, ad-free engine for browsing tools.
🤖 LM Studio: The best way to run local LLMs.
🛠️ Installation & Setup Guide
Follow these steps carefully to get your local tool-calling assistant up and running!
Step 1: Download the Model
Open LM Studio and search for the tool-calling model.
Download: Gemma 4 (Make sure to grab the appropriate quant for your system, e.g., Q4 or Q8).
Step 2: Configure Your Details
Before uploading the configuration files to LM Studio, you need to personalize them:
Open the .json tool configuration file provided in this repo.
Find the "username": "YOUR_USERNAME_HERE" field.
Add your username to replace the placeholder and save the file.
Step 3: Import Configs to LM Studio
Now, let's inject the tools into LM Studio:
Navigate to the Developer / Tools section in LM Studio.
Upload the .json file you just edited. This defines the tool structures (like the Brave browser integration).
Copy the System Prompt from this repo (system_prompt.txt) and paste it into the System Prompt configuration box in LM Studio. (This tells Gemma 4 how and when to use the tools).
Step 4: Reboot
For the changes to fully take effect and for the tool schemas to register:
🔄 Restart LM Studio completely (Close the app and open it again).
🧪 Testing it Out
Once LM Studio is back up, load your Gemma 4 model and paste the following into the chat to test if the tools are working properly:
LLM Test Prompt:
"Use the Brave browser tool to search for the current weather in Tokyo and summarize the top 3 results for me."
If everything is configured correctly, Gemma 4 will trigger the tool, process the JSON, and return a real-time answer!
🎉 Enjoy!
You now have a fully functional, local, tool-calling AI. Feel free to tweak the system prompt and add more tools to the JSON file to expand your assistant's capabilities.
If you like this project, don't forget to ⭐ star the repo!

