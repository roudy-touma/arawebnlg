# arawebnlg

This repository contains codes and dataset for the ACM TALLIP paper titled "Automated Generation of Human-readable Natural Arabic Text from RDF Data".

The work builds on state-of-the-art techniques in Natural Language Processing (NLP) for Arabic, leveraging pre-trained models like **AraBERT** and **AraGPT2** to perform data-to-text generation tasks. 

The dataset used focuses on generating Arabic text for various domains, including sports, politics, and arts.

## Dataset

The dataset used in this project is the **AraWebNLG 2020** dataset, containing data from categories such as:
- **SportsTeam**
- **CelestialBody**
- **Food**
- **Artist**
- **University**
- **Politician**

Each data point contains an Arabic RDF input data (`input_text_ar`) and its corresponding target sentence (`target_text_ar`).

---

## Model Architecture

The core architecture used in this repository is an encoder-decoder model (sequence-to-sequence). Specifically relying on the pretrained transformer architectures:

- AraBERT (`aubmindlab/bert-base-arabert`)
- AraGPT2 (`aubmindlab/aragpt2-base`)
- mT5 (`google/mt5-base`)

---

## Reference
For more details on the implementation and results, refer to the related paper [here](https://dl.acm.org/doi/abs/10.1145/3582262).

If you use this repository in your research, please consider citing the paper:

```
@article{10.1145/3582262,
    author = {Touma, Roudy and Hajj, Hazem and El-Hajj, Wassim and Shaban, Khaled},
    title = {Automated Generation of Human-readable Natural Arabic Text from RDF Data},
    year = {2023},
    issue_date = {April 2023},
    publisher = {Association for Computing Machinery},
    address = {New York, NY, USA},
    volume = {22},
    number = {4},
    issn = {2375-4699},
    url = {https://doi.org/10.1145/3582262},
    doi = {10.1145/3582262},
    journal = {ACM Trans. Asian Low-Resour. Lang. Inf. Process.},
    month = mar,
    articleno = {98},
    numpages = {13},
    keywords = {datasets, neural networks, language models, RDF, data-to-text, Low-resource languages}
}
```