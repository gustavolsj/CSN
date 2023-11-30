# CSN - Collection Space Navigator: 
An Interactive Visualization Interface for Multidimensional Datasets   
[Repository: https://github.com/Collection-Space-Navigator/CSN](https://github.com/Collection-Space-Navigator/CSN)  

![CSN: Collection Space Navigation](./fig1_web.png) 

The Collection Space Navigator (CSN) is an explorative visualization tool for researching collections and their multidimensional representations. We designed this tool to better understand multidimensional data, its methods, and semantic qualities through spatial navigation and filtering. CSN can be used with any image collection and can be customized for specific research needs (see Jupyter Notebook or Google Colab).

The CSN code is partly based on the [umap-explorer](https://github.com/GrantCuster/umap-explorer) by [GrantCuster](https://github.com/GrantCuster).

# Project Links
[🖥️ Online demo](https://collection-space-navigator.github.io/CSN)    
[📄 Paper on arxiv.org](http://arxiv.org/abs/2305.06809)  
[🌐 Project website](https://collection-space-navigator.github.io)  


## Getting Started
We recommend using our colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Collection-Space-Navigator/CSN/blob/main/CSN_colab.ipynb). It prepares the datasets and build a customized version of the Collection Space Navigator. For Jupyter Notebook, please use `CSN_notebook.ipynb`

## Using the Collection Space Navigator
Place your prepared dataset folders in the `build/datasets` directory and modify `build/datasets/datasets_config.json`. We recommend using our colab `CSN_colab.ipynb` to format your data correctly.

To use the Collection Space Navigator locally run:
```
serve -s build
```
The CSN should be now accessible at `http://localhost:3000` in your browser.


## Development 
*For development only.*     

Required: <a href="https://nodejs.org/en/download" target="_blank">node.js</a>  


Important: `node 16.16.0` is required! We recommend using <a href="https://github.com/nvm-sh/nvm" target="_blank">NVM</a>   for node version managing:
```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" # This loads nvm
nvm install v16.16.0
```
In the `CSN` directory, run:
```
npm install
```
To run the development server:
```
npm start
```   
Open [http://localhost:3000](http://localhost:3000) to view in your browser.

For production, run:
```
npm run build
```
It bundles React in production mode and optimizes the build for the best performance.    
    
The build is minified and the filenames include the hashes.    
Your app is ready to be deployed!    
    
See the section about <a href="https://facebook.github.io/create-react-app/docs/deployment" target="_blank">deployment</a> for more information.

## Citation
```
@misc{ohm2023collection,
      title={Collection Space Navigator: An Interactive Visualization Interface for Multidimensional Datasets}, 
      author={Tillmann Ohm and Mar Canet Solà and Andres Karjus and Maximilian Schich},
      year={2023},
      eprint={2305.06809},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```

## Authors
<a href="https://tillmannohm.com/" target="_blank">Tillmann Ohm</a>, 
<a href="https://var-mar.info/" target="_blank">Mar Canet Solà</a>

## Gallery examples using CSN
* Kinokroonika project CSN - Visualizing Estonian newsreels in the 20th century: <a href="https://csn.kinokroonika.ee/" target="_blank">https://csn.kinokroonika.ee/</a>

If you have used CSN it in your project, email us, and we will publish it here.

## Acknowledgements
Tillmann Ohm and Mar Canet Solà designed, co-authored, and developed the Collection Space Navigator (CSN) software. <a href="https://tillmannohm.com/" target="_blank">Tilmann Ohm</a>, <a href="https://var-mar.info/" target="_blank">Mar Canet Solà</a>, <a href="https://andreskarjus.github.io"  target="_blank">Anders Karjus</a>, <a href="https://www.schich.info/"  target="_blank">Maximilian Schich</a> contributed to the broader research design, including initial applications of the CSN. The authors further thank the members of the CUDAN Research Group for useful discussions. All authors are supported by ERA Chair for <a href="https://cudan.tlu.ee/" target="_blank">Cultural Data Analytics</a>, funded through the European Union’s Horizon 2020 research and innovation program (Grant No.810961).
