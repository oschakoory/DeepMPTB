<img align="right" src="datas/logo.png" width="150" alt="DeepMPTB logo"/>

# DeepMPTB
![GitHub](https://img.shields.io/github/license/oschakoory/RiboTaxa)
![GitHub](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Foschakoory%2FDeepMPTB&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=views&edge_flat=true)

If you use DeepMPTB in your work, please cite the DeepMPTB paper:

Oshma Chakoory, Vincent Barra, Emmanuelle Rochette, Loïc Blanchon, Vincent Sapin, Etienne Merlin, Maguelonne Pons, Denis Gallot, Sophie Comtet-Marre & Pierre Peyret. DeepMPTB: a vaginal microbiome-based deep neural network as artificial intelligence strategy for efficient preterm birth prediction. Biomark Res 12, 25 (2024). https://doi.org/10.1186/s40364-024-00557-1 

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
