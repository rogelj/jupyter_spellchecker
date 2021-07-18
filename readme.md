# Spellcheck Jupyter Notebooks

If you are interested in getting some spellchecking capabilities in the markdown cells of your Jupyter notebookm take a look at these instrucctions. 

1. Install Jupyter notebook extensions ([nbextensions](https://github.com/ipython-contrib/jupyter_contrib_nbextensions)). This includes [Spellchecker](https://nicoguaro.github.io/posts/ortografia_jupyter/.) and a that is the extension we are after in this case.

   Type the following in a terminal, to install it using PIP.

   ```zsh
   pip install jupyter_contrib_nbextensions
   ```

   However, if Anaconda is being used the **recommended method** is to use `conda`, as shown below.

   ```zsh
   conda install -c conda-forge jupyter_contrib_nbextensions
   ```

   When you start your Jupyter notebook you will see a new tab: The [configuration interface](https://github.com/Jupyter-contrib/jupyter_nbextensions_configurator). In the main menu of Jupyter notebook a new tab named *Nbextension* will appear. 

2. You need to get hold of suitable dictionaries in UTF-8 encoding. I am including some en British English and Spanish (Spain and Mexico) in this repo. 

   Download the files and place them in the following directory

   ```zsh
   ~/.local/share/jupyter/nbextensions/spellchecker/typo/dictionaries
   ```

   Note that the directory above depends on your actual installation. For instance you may find that with Anaconda on a mac you will need to place the files in the following path:

   ```zsh
   /Applications/anaconda3/share/jupyter/nbextensions/spellchecker/typo/dictionaries
   ```

3. Point the extension to the correct path. For the British English dictionaries use the following configuration:

   - Language code for typo.js: `en_GB`

   - Dictionary .dic file: `./typo/dictionaries/en_GB.dic`

   - Dictionary .aff file: `./typo/dictionaries/en_GB.aff`

   For the Spanish (Spain) ones:

   - Language code for typo.js: `es_ES`
   - Dictionary .dic file: `./typo/dictionaries/es_ES.dic`
   - Dictionary .aff file: `./typo/dictionaries/es_ES.aff`

   For the Spanish (Mexico) ones:
   
   - Language code for typo.js: `es_MX`
   
   - Dictionary .dic file: `./typo/dictionaries/es_MX.dic`
   
   - Dictionary .aff file: `./typo/dictionaries/es_MX.aff`

More dictionaries are available from: https://github.com/wooorm/dictionaries

