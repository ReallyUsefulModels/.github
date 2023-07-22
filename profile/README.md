## Hi there 👋

🙋‍♀️ Welcome to Really Useful Models or RUM. Our not-for-profit mission is to bring open-source system dynamics modelling to the world and particularly the NHS.<br />

System Dynamics (SD) in the NHS is a bit of a dark art. I found it very hard when it was first explained to me. There is also an idea that it is somehow not useful compared to machine learning but this is incorrect - both are useful. Both Wang and Matt are pretty good at machine learning but they also both love SD. This is why they created ASDM or Agile System Dynamics Modelling.

Wang was the first to realize that there was a need for a new framework. PySD is great for newcomers but as soon as SD models get complicated it falls over, as do the other frameworks out there. Python is not a quick language so he has spent a lot of time improving its speed and balancing this with accessibility. It is designed such that machine learning inputs or outputs can be subsequently added but the core focus is on having a really robust SD engine with support for complex arrays. 

Matt has spent a lot of time experimenting with Streamlit and ways to deploy the software fully open source without scale penalty in a way that people within the NHS can access. Making the frontend more accessible and testing the backend to make it more robust has been his main focus. Now it is finally ready for the world to start trying it out.

We have very much been working this out iteratively over time but the core focus is making it easier to openly deploy useful models in a non-arcane/scary way. There is a bit of coding involved but we aim to keep this as simple as possible and simplify it further over time. The even better news these days is that if you are not a coder you can just use chatGPT (or another GPT model of your choice - BARD/Llama2 if you prefer open source to work out how to build and deploy the apps. 

Matt has also written a guide to getting started with Python here: https://mattstammers.github.io/hdruk_avoidable_admissions_collaboration_docs/how_to_guides/new_to_python/

🌈 Contribution guidelines - You can get involved by submitting pull requests, ideas or just sending us a message.<br />

Please feel free to contribute or upload any models you have. We recommend using streamlit cloud to deploy them, which can be found here: https://streamlit.io/. Here is an example model deployed on the platform: https://donanumabmodel.streamlit.app/

To set the environment up to start coding clone a template app using for example:

```sh
git clone https://github.com/ReallyUsefulModels/Donanumab_Model.git
```

Then make sure pipenv is installed:

```sh
pip install pipenv
```
Followed by:

```sh
pipenv install
```

Then to start the shell call
```sh
pipenv shell
```

And you can either launch a juptyer-lab notebook from here or run the program in any development environment you choose. We recommend VScode for those without a strong preference. 

- Hints:
1. Use the notebook to start developing as it will allow you to iterate and test out ideas
2. When you are happy with your model try to deploy it locally in the browser using streamlit by calling

```python
streamlit run {name_of_file.py}
```

3. Focus on usability in the design of your app. When you are ready to deploy it you can do so using the Streamlit cloud service. 

👩‍💻 Useful resources - The PyPI repository for ASDM can be found here: (https://pypi.org/project/asdm/). Here you will also find the ASDM setup guide.<br />

🧙 What's Coming Next? The first Python SD models are now available, with more to follow. Watch this space. If you want to give feedback, please do. The best way is to lodge an issue on a repository explaining the problem and we will do our best to try and address it. 

