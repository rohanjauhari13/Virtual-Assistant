# Virtual-Assistant
A Covid and weather tracker chatbot built in RASA that understands complex queries in natural language. Fetches data via API.

actions.py is the dialogue engine. The dialogue flow has been coded in python.

Intents and Entities are in data folder.

Trained models will be stored in models folder.

domain file has declaration of every intent, entity, slot, story and action used.

Rasa runs on local console like python.

To connect it to another software development framework, we need to first run it on some server and then query it using that server's API from our application.
We run rasa on localhost:5005 by command "rasa run".

The API for quering rasa bot running on localhost:5005 is "https://localhost:5005/webhooks/rest/webhook". But as it's localhost, this api will only work from the same computer. To
access chatbot from another computer, use ngrok.

Chatbot can also be accessed via external channels like Telegram, MatterMost, FB messenger, Slack, Twilio etc via credentials file.
