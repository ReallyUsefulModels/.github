## Welcome to Really Useful Models (RUM) 👋

🙋‍♀️ Welcome to Really Useful Models or RUM. Our not-for-profit mission is to bring open-source system dynamics modelling to the world and particularly the NHS.<br />

System Dynamics (SD) in the NHS is a bit of a dark art. I (Matt) found it very hard when it was first explained to me. There is also an idea that it is somehow not useful compared to machine learning but this is incorrect - both are useful. The creators of this repo (primarily Wang Zhao and Matt Stammers) are pretty good at machine learning but they also both love SD. This is why they created ASDM or Agile System Dynamics Modelling.

Wang was the first to realize that there was a need for a new framework and had been working on ASDM for a while. PySD is great for newcomers and highly accessible but the compiler doesn't work for very complex models out of the box. Python is not a quick language so Wang spent a lot of time improving its speed and balancing this with accessibility. It is designed such that machine learning inputs or outputs can be subsequently added but the core focus is on having a really robust SD engine with support for complex arrays. 

Matt has spent a lot of time experimenting with Streamlit and ways to deploy the software fully open source without scale penalty in a way that people within the NHS can access. Making the frontend more accessible, the backend more robust, and adding some dev-ops and product design to the process has been his focus. After around a year of tinkering, it is finally ready for the world to start trying it out properly. 

There is a bit of coding involved but we aim to keep this as simple as possible and simplify it further over time. The even better news these days is that if you are not a coder you can use chatGPT (or another GPT model of your choice - BARD/Llama2 if you prefer open source to work out how to build and deploy apps yourself.

Matt has also written a guide to getting started with Python here which was originally written for a HDRUK project but is also suitable for those wishing to use ASDM https://mattstammers.github.io/hdruk_avoidable_admissions_collaboration_docs/how_to_guides/new_to_python/

🌈 Contribution guidelines - You can get involved by submitting pull requests, ideas or just sending us a message.<br />

Please feel free to contribute or upload any models you have. We recommend using streamlit cloud to deploy them, which can be found here: https://streamlit.io/. The available example models are listed at the bottom. Obviously don't share anything which needs to be protected but any open-source models can easily be deployed here using streamlit cloud. 

### Getting Started

If you have done a bit of programming before it should be easy. To set the environment up to start coding clone a template app using for example:

```sh
git clone https://github.com/ReallyUsefulModels/Smoking_Cessation_Training.git
```

or click on the repository and create a new repository using the template of your choice (described more below).

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

#### Hints:
1. Use the notebook to start developing as it will allow you to iterate and test out ideas
2. When you are happy with your model try to deploy it locally in the browser using streamlit by calling

```python
streamlit run {name_of_file.py}
```

3. Focus on usability in the design of your app. When you are ready to deploy it you can do so using the Streamlit cloud service. 

👩‍💻 Useful resources - The main PyPI repository for ASDM can be found here: (https://pypi.org/project/asdm/). Here you will also find the ASDM setup guide.<br />

#### Recommended External Resources
There are also some very useful online SD resources available such as: 

- https://github.com/JimDuggan/SDMR. For R lovers.
- https://github.com/SDXorg/SD-Tools. We are not on this list yet but hopefully will be soon.
- https://pysd.readthedocs.io/en/master/index.html. If you want a mature framework for open-source SD modelling we recommend you check out PySD. Some of the models here will not work with it but PySD is easier for beginners to pick up. ASDM is a complex-model handling framework but PySD can easily handle all the simple models. If you get stuck please don't give up, instead check out PySD.

🧙 If you want to give feedback, please do. The best way is to lodge an issue on a repository explaining the problem and we will do our best to try and address it. We have three models live currently of 3 levels of complexity and difficulty to learn.

1. Introductory: https://smokingcessation.streamlit.app/ - This repository features the tutorial and is easy for even those new to SD to get their heads around.
2. Moderate: https://electiverecovery.streamlit.app/ - This repository features the NHS elective recovery model which is fairly complicated and takes a bit of thinking to understand. However, it features a mini notebook tutorial to introduce users to some of the more complex elements of ASDM.
3. Advanced: https://donanumabmodel.streamlit.app/ - This repository features the donanumab model (a new anti-dementia drug). The model introduces users to graph functions and networkx digraphs so is recommended for users used to using ASDM.

### How to Use Templates

These three notebooks serve as the base templates. For new members or users using ASDM for the first time we recommend cloning or using the smoking cessation template to get started. Just go to this URL: https://github.com/ReallyUsefulModels/Smoking_Cessation_Training/tree/main and click use this template to create a new repository from the base template.

It is generally best to develop on your own local machine so once you have named your repository you should call:

```git
git clone [name of repository.git]
```

If you click the clone button it will give you the link you need to clone the repository. Then you can code on your local machine. To create a branch call:

```git
git checkout -b "[name of new branch]"
```

Then you can call ```git add .``` and ```git commit -m "message"``` as needed while you are developing. When you are finished call:

```git
git push
```

The first time you do this you will need to set the upstream branch but then all your work will be stored in the RUM repository branch and can be merged to main when finished. To test Streamlit locally you just need to call this and it will run in your local browser:

```python
streamlit run [name_of_app.py]
```
Good luck! If you are not a member yet or get another issue just email us at the email address above 😊. The aim is for this to be an open and inclusive community of SD modellers.

Happy Coding! 🙌
