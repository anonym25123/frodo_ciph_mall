# frodo_ciph_mall
## Description
Python source code (Jupyter Notebook) to exploit ciphertext malleability against the post-quantum cryptography primitive FrodoKEM. This source allows to study three different approaches to the choice of alterations to a ciphertext message. The alterations impact the secret message value during the decrpytion and are supposedly recovered thanks to a Side-Channel Oracle.

In this work, we assume the Oracle outputs the Hamming Weight of the secret message. The different attack strategies are as follows:
- Direct approach (funciton straight_attack), where a set of biases to test is pre-determined before the attack,
- Adaptive approach (function adaptive_attack), where the next tested bias depends on the results of the lattest,
- Brute-force approach (function average_recovery), where only one bias is chosen and the remaining secret message bits are brute-forced.

## Requirements
This notebook must be run in a Jupyter environment. An online envrionment is available with the [Jupyter Lite demo](https://jupyterlite.github.io/demo/lab/index.html). 

## Usage
1. Download the notebook either directly or by cloning the repository
   ```shell
   git clone https://github.com/anonym25123/frodo_ciph_mall.git
   ```
2. Open the  [Jupyter Lite demo](https://jupyterlite.github.io/demo/lab/index.html).
3. Upload the Frodo_attack.ipynb file in the demo.
   
   ![upload in Jupyter Lite](https://github.com/anonym25123/frodo_ciph_mall/blob/main/upload.gif)
   
4. Select the notebook in the files menu by double-clicking it.
   
   ![select in Jupyter Lite](https://github.com/anonym25123/frodo_ciph_mall/blob/main/notebook.gif)
   
5. The notebook is ready. Use **Shift+Enter** to execute the notebook cells one after the other.

## Folder content
- *Frodo_attack.ipynb*: The Jupyter Notebook with the source code.
- *LICENSE*: MIT License.
- *README.md*: This file.
- *notebook.gif* and *upload.gif*: Images for the README.md file
