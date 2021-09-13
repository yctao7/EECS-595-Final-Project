# Verifiable-Coherent-NLU
Shared repository for TRIP dataset for verifiable NLU and coherence measurement for text classifiers. Covers the following upcoming publications in Findings of EMNLP 2021:
1. Shane Storks, Qiaozi Gao, Yichi Zhang, and Joyce Chai. (2021). [Tiered Reasoning for Intuitive Physics: Toward Verifiable Commonsense Language Understanding](https://arxiv.org/abs/2109.04947). In _Findings of EMNLP 2021_.
2. Shane Storks and Joyce Chai. (2021). [Beyond the Tip of the Iceberg: Assessing Coherence of Text Classifiers](https://arxiv.org/abs/2109.04922). In _Findings of EMNLP 2021_.

Please contact [Shane Storks](http://scr.im/sstorks) with any questions.

## Getting Started

Our results can be reproduced using the Python notebook file [Verifiable-Coherent-NLU.ipynb](Verifiable-Coherent-NLU.ipynb), which we ran in Colab (may require some adaptation for use in Jupyter).

Clone the repo:
```
git clone https://github.com/sled-group/Verifiable-Coherent-NLU.git
```

You will then need to upload the contents of this folder to Google Drive.

From the `Verifiable-Coherent-NLU` directory in your Google Drive, open [Verifiable-Coherent-NLU.ipynb](Verifiable-Coherent-NLU.ipynb) using [Google Colab](https://colab.research.google.com).

## Reproducing Results

Configure the cells below the first heading of [Verifiable-Coherent-NLU.ipynb](Verifiable-Coherent-NLU.ipynb) as needed and run the **Setup** block to prepare the notebook for reproducing a specific set of results. Then navigate to the appropriate block to reproduce results on TRIP, Conversational Entailment, or ART. Each block will have sub-blocks for preparing the data (run every time), and for training and testing models.

You may either re-train the models from the papers, or use our pre-trained model instances (see below).

### Pre-Trained Model Instances
Pre-trained model instances from the paper are available [here](https://drive.google.com/file/d/1rOTzGSI33D0Wp1sy048dmQcwIDODJIz_/view?usp=sharing). Copy the archive file to your own Google Drive, and unzip into a new directory `./saved_models`, then run inference on them as needed using the appropriate blocks in the notebook. The names of the provided pre-trained model directories are already listed in the configuration area for convenience.

## Cite
If you use our code or models in your work, please cite one of our following papers (both accepted to Findings of EMNLP 2021):
```
  @misc{storks2021tiered,
        title={Tiered Reasoning for Intuitive Physics: Toward Verifiable Commonsense Language Understanding}, 
        author={Shane Storks and Qiaozi Gao and Yichi Zhang and Joyce Chai},
        year={2021},
        eprint={2109.04947},
        archivePrefix={arXiv},
        primaryClass={cs.CL}
  }
```

```
  @misc{storks2021tip,
        title={Beyond the Tip of the Iceberg: Assessing Coherence of Text Classifiers}, 
        author={Shane Storks and Joyce Chai},
        year={2021},
        eprint={2109.04922},
        archivePrefix={arXiv},
        primaryClass={cs.CL}
  }
```

Additionally, please consider citing [Conversational Entailment](https://sled.eecs.umich.edu/post/resources/conversation-entailment/) and [ART](https://github.com/allenai/abductive-commonsense-reasoning), which are used in experiments from the latter paper (and included in this repo):
```
  @inproceedings{zhang-chai-2010-towards,
      title = "Towards Conversation Entailment: An Empirical Investigation",
      author = "Zhang, Chen  and
        Chai, Joyce",
      booktitle = "Proceedings of the 2010 Conference on Empirical Methods in Natural Language Processing",
      month = oct,
      year = "2010",
      address = "Cambridge, MA",
      publisher = "Association for Computational Linguistics",
      url = "https://aclanthology.org/D10-1074",
      pages = "756--766",
  }
```

```
  @inproceedings{
      bhagavatula2020abductive,
      title={Abductive Commonsense Reasoning},
      author={Chandra Bhagavatula and Ronan Le Bras and Chaitanya Malaviya and Keisuke Sakaguchi and Ari Holtzman and Hannah Rashkin and Doug Downey and Wen-tau Yih and Yejin Choi},
      booktitle={International Conference on Learning Representations},
      year={2020},
      url={https://openreview.net/forum?id=Byg1v1HKDB}
  }
```
