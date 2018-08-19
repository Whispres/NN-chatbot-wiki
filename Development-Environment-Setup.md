# Development Environment Setup
## Operating System Compatibility
NN-chatbot is built in Java and Python with no specific  operating system (OS) formatting. The program is designed to be universally compatible with any OS platform, but has only been validated in Windows.

Volunteers interested in OS platform validation are needed and appreciated! Review the contribution guidelines in the CONTRIBUTING.md file. To report compatibility errors, open an issue on the NN-Chatbot Github page [here](https://github.com/LunarWatcher/NN-chatbot/issues).

## Chatbot Prerequisites
Click on the program name to be redirected to the respective download/installation page.

#### [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
* Git must be available from a command prompt for the revision command to work.
* Recommended: Install and add Git to the PATH environment variable.

#### [Gradle](https://gradle.org/install/)
* This is the build tool designed to automate the build process and support multi-language development.
* See the [Gradle Github page](https://github.com/gradle/gradle) or the [Gradle website](https://gradle.org) for more details.

#### [IntelliJ](https://www.jetbrains.com/idea/download/#section=windows)
* Supports Python editing with the [Python plugin](https://www.jetbrains.com/help/idea/plugin-overview.html).
* IntelliJ IDEA projects can be synchronized with Gradle projects, and IntelliJ IDEA can configure a Gradle composite build. For more information, click [here](https://www.jetbrains.com/help/idea/gradle.html).
* **NOTE:** [PyCharm](https://www.jetbrains.com/pycharm/download/#section=windows) is a viable alternative to IntelliJ if the Java port is not used, but it cannot synchronize with Gradle. Also, the Python plugin for IntelliJ IDEA has the same functionality as the community edition of PyCharm, so it is possible to continue working from IntelliJ even without the Java port. This is why using IntelliJ in conjunction with Gradle is preferable.

#### [Python 3.6+](https://www.python.org/downloads/)
* **NOTE:** Python 3.6+ is only necessary if the NN module/Python bot is used.

#### [Java 8](https://java.com/en/download/)
* **NOTE:** Java 8 is only necessary if the Java port is used.

## Clone the Repository
#### Clone by Command Prompt
Use the command prompt to clone the repository and cd into the NN-chatbot directory.
```
git clone https://github.com/LunarWatcher/NN-chatbot.git
cd NN-chatbot
```
## Dataset

The [Cornell Movie-Dialogs Corpus](http://www.cs.cornell.edu/~cristian/Cornell_Movie-Dialogs_Corpus.html)

The bot is currently designed for this dataset. There will be support for custom dataset (and conversation scraping for personalized conversations) at a later date.

* Download the ZIP file and extract the dialogue text files into the `raw_data` directory.
<!--Where is the raw_data directory? Does the user need to make one? Where does the raw_data directory go in the repository?-->

## Java/Kotlin Bot Dependencies

The Java/Kotlin bot dependencies are defined in the build system. Gradle automatically downloads the dependencies for the Java bot.

## Python Neural Network Dependencies

**NOTE:** The Java/Kotlin bot interfaces with the Python neural network, but is not dependent on it. The following is only required if the bot will be set to use the neural network.

The recommended versions of each dependency are also listed in [`requirements.txt`](https://github.com/LunarWatcher/NN-chatbot/blob/master/requirements.txt).

[pytest](https://docs.pytest.org/en/latest/) - A Python testing tool.

[NumPy](http://www.numpy.org/) - A package for scientific computing with Python.

[Natural Language Toolkit (NLTK)](https://www.nltk.org/) - A platform for writing Python programs which use human language data.

[discord.py](https://github.com/Rapptz/discord.py) - The API wrapper for Discord written in Python.

[Setuptools](https://setuptools.readthedocs.io/en/latest/) - A library for packaging Python projects.

[Requests](http://docs.python-requests.org/en/master/) - An HTTP library for Python.

[Tensorflow](https://www.tensorflow.org/) - The machine learning framework.
* There are two versions of TensorFlow: TensorFlow with CPU support only and TensorFlow with GPU support (aka: tensorflow-gpu). TensorFlow with GPU support is better suited for neural networks and/or machine learning, but both versions are acceptable.
* See the TensorFlow [official installation guide](https://www.tensorflow.org/install/) for details.

[Tensorlayer](https://github.com/tensorlayer/tensorlayer) - A Deep Learning (DL) and Reinforcement Learning (RL) library.
* TensorLayer has several prerequisites which may require the `pip install` command to complete the installation.
* See the TensorLayer [official installation guide](http://tensorlayer.readthedocs.io/en/latest/user/installation.html) for details.

[Tensorboard](https://www.tensorflow.org/guide/summaries_and_tensorboard) - Visualization toolkit for working with Tensorflow.

[httmock](https://github.com/patrys/httmock) - A mocking library for testing requests.

[Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) - A Python library for extracting data from HTML and XML files.

[Scikit-Learn](http://scikit-learn.org/stable/) - A machine learning library for Python.

[Websocket Client](https://github.com/websocket-client/websocket-client) - A Websocket client for Python.

[asyncio](https://docs.python.org/3/library/asyncio.html) - A module providing infrastructure for writing  asynchronous I/O, event loop, coroutines and tasks.
 <!--Listed in the README but not in the requirements.txt...-->

## Ready?
Do you have your Stack Exchange, Discord and/or Twitter bot account information?
  - See examples of how the account information is used in  [`bot.properties-example`](bot.properties-example.md), [`creds.properties-example`](creds.properties-example.md), [`Config.py_example`](Config.py_example.md).
  * See [Bot Account Registration Help](Bot-Account-Registration-Help.md) for more on registering accounts and finding account information.

Once all programs/dependencies are downloaded and installed, proceed to [Setting up the bot](Setting-up-the-bot.md).
<!--Unsure if they should be redirected to the Setting-up-the-bot wiki page or the Readme. Add a link later.-->
