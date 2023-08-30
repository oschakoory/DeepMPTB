<img align="right" src="datas/logo.png" width="150" alt="DeepMPTB logo"/>

# DeepMPTB

DeepMPTB can directly be accessed here: https://deepmptb.streamlit.app/

# Running the application locally
Step 1: Install docker - follow this link https://docs.docker.com/engine/install/ubuntu/ </br>
Step 2: Download this projet </br>
Step 3: On the docker terminal, go to the root directory of this projet where you can see the file Dockerfile </br>
Step 4: Execute this command to build your docker image </br>
&nbsp;&nbsp;<h4>docker build -t deepmptb</h4></br>
Step 5: Execute this command to run the application locally </br>
&nbsp;&nbsp;<h4>docker run -p 8501:8501 deepmptb</h4></br>
</br>
Using the browser of your choice, you can access the application at http://localhost:8501 </br>
</br>

## DeepMPTB for prediction

DeepMPTB needs
- Taxonomic profile table (see datas/ERR10897566_SSU_taxonomy_abundance.tsv as an example)
- Ethnicity of woman
- Age of woman 
- Trimester of sample collection

The taxonomic profiles are produced by <a class="reference external" href="https://github.com/oschakoory/RiboTaxa" target="_blank" rel="noopener noreferrer">RiboTaxa</a>, a metagenomics classifier for precise species level identification from shotgun metagenomics.

In case if the three clinical data are not available, users can choose "unknown" for each data.
