# **LatexToolkit** 📝 → 📄  

**LatexToolkit** is lightweight Python package working on top of [magic-pdf](https://github.com/opendatalab/MinerU). It is designed to convert documents into **LaTeX** format. Whether you're working with PDFs, markdown files, or other structured text formats, this toolkit is thought to streamline the workflow of LaTeX conversion.  

## **Features**   
✔️ End to end pipeline from PDF to LaTeX .  
✔️ LaTeX commands supported: section{}, figures, equations,	tables, and inline math.  


Future features: Support of .doc , .docx , .ppt and .pptx. formats.

## **Installation** 

### 1. Ensure to install first magic-pdf

Using Conda env:

```sh
conda create -n MinerU python=3.10
conda activate MinerU
pip install -U magic-pdf[full] --extra-index-url https://wheels.myhloli.com
```

Download model weight files:

```sh
pip install huggingface_hub
wget https://github.com/opendatalab/MinerU/raw/master/scripts/download_models_hf.py -O download_models_hf.py
python download_models_hf.py
```

If using GPU [follow magic-pdf Official installation](https://mineru.readthedocs.io/en/latest/user_guide/install/boost_with_cuda.html)


### 2. Install **LatexToolkit** via pip:  

```sh
pip install LatexToolkit
```

## **Ussage** 

Run the tool from the terminal to convert a document:

```sh
latex_toolkit input_file.pdf
```

or use it in your Python scripts:

```sh

from LatexToolkit import to_latex

to_latex("input_file.pdf")
```


