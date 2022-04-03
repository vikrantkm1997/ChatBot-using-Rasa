1. First create environment which was done in vikenv
   python -m venv vikenv
Now enter the environment vikenv
   vikenv\Scripts\activate
2. install modules
pip install tensorflow
pip install rasa
python -m spacy link en_core_web_md en

Now go to config.yml
and replace language : en with language: en_core_web_md
This is done to link spacy

3. go to cmd where  this environment is created
   rasa init
   //Enter path
   y
   y
   n

4. Define intents in nlu.md, in domain.yml add intents and corresponding output
   In stories.md we have the intents and its output(we are defining the flow of converation)

5. go inside chatbot folder here cb1, run cmd and train the model by commad
   rasa train
   after training to start the model type 
   rasa shell
   This will start the chatbot in local server