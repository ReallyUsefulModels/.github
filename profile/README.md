## Hi there 👋

🙋‍♀️ Welcome to Really Useful Models or RUM. Our not-for-profit mission is to bring open-source system dynamics modelling to the world.<br />

🌈 Contribution guidelines - You can get involved by submitting pull requests, ideas or just sending us a message.<br />

Please feel free to contribute or upload any models you have. We recommend using streamlit cloud to deploy them, which can be found here: https://streamlit.io/ 

If you are not a coder, we recommend using a GPT chat model of your choice to work out how to build and deploy the apps. We have written a guide to getting started with Python here: https://mattstammers.github.io/hdruk_avoidable_admissions_collaboration_docs/how_to_guides/new_to_python/

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

🧙 What's Coming Next? The first Python SD models are now available with more to follow. Watch this space

