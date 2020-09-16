# Dialog State Tracking Challenge 2 &amp; 3 Data

*This data used to be hosted on http://camdial.org/~mh521/dstc/*

## Data downloads

* [handbook.pdf](handbook.pdf) - The DSTC 2 & 3 Handbook with information about the data formats used
* [dstc2_traindev.tar.gz](https://github.com/matthen/dstc/releases/download/v1/dstc2_traindev.tar.gz) - Train and development datasets for DSTC 2.
* [dstc2_test.tar.gz](https://github.com/matthen/dstc/releases/download/v1/dstc2_test.tar.gz) -  Test dataset for DSTC 2.
* [dstc3_seed.tar.gz](https://github.com/matthen/dstc/releases/download/v1/dstc3_seed.tar.gz) - Labeled seed dataset for DSTC 3.
* [dstc3_test.tar.gz](https://github.com/matthen/dstc/releases/download/v1/dstc3_test.tar.gz) - Test dataset for DSTC 3.
* [dstc2_scripts.tar.gz](https://github.com/matthen/dstc/releases/download/v1/dstc2_scripts.tar.gz) - Evaluation scripts, baseline tracker and other tools.
* [HWU_baseline.zip](https://github.com/matthen/dstc/releases/download/v1/HWU_baseline.zip) - Alternative baseline tracker, provided by Zhuoran Wang.

Original challenge results:

* [dstc2_results.zip](https://github.com/matthen/dstc/releases/download/v1/dstc2_results.zip) - Full results of the DSTC 2.
* [dstc2_results_small.zip](https://github.com/matthen/dstc/releases/download/v1/dstc2_results_small.zip) - Results for the DSTC 2, not including tracker outputs.
* [dstc3_results.zip](https://github.com/matthen/dstc/releases/download/v1/dstc3_results.zip) - Full results of the DSTC 3.
* [dstc3_results_small.zip](https://github.com/matthen/dstc/releases/download/v1/dstc3_results_small.zip) - Results for the DSTC 3, not including tracker outputs.


## Overview


The Dialog State Tracking Challenges 2 &amp; 3 (DSTC2&amp;3) were research challenge focused on improving the state of the art in tracking the state of spoken dialog systems. State tracking, sometimes called belief tracking, refers to accurately estimating the user's goal as a dialog progresses. Accurate state tracking is desirable because it provides robustness to errors in speech recognition, and helps reduce ambiguity inherent in language within a temporal process like dialog.


In these challenges, participants were given labelled corpora of dialogs to develop state tracking algorithms. The trackers were then evaluated on a common set of held-out dialogs, which were released, un-labelled, during a one week period.

The corpus was collected using Amazon Mechanical Turk, and consists of dialogs in two domains: restaurant information, and tourist information. Tourist information subsumes restaurant information, and includes bars, cafés etc. as well as multiple new slots. There were two rounds of evaluation using this data:

* **DSTC 2** released a large number of training dialogs related to restaurant search. Compared to DSTC (which was in the bus timetables domain), DSTC 2 introduces changing user goals, tracking 'requested slots' as well as the new restaurants domain. Results from DSTC 2 were presented at SIGDIAL 2014.
* **DSTC 3** addressed the problem of adapation to a new domain -- tourist information. DSTC 3 releases a small amount of labelled data in the tourist information domain; participants will use this data plus the restaurant data from DSTC 2 for training.

Dialogs used for training are fully labelled; user transcriptions, user dialog-act semantics and dialog state are all annotated. (This corpus therefore is also suitable for studies in Spoken Language Understanding.)

For more detailed information, please see the [handbook](handbook.pdf).


# Citations

```bibtex

@inproceedings{henderson2014second,
  title={The second dialog state tracking challenge},
  author={Henderson, Matthew and Thomson, Blaise and Williams, Jason D},
  booktitle={Proceedings of the 15th annual meeting of the special interest group on discourse and dialogue (SIGDIAL)},
  pages={263--272},
  year={2014}
}

@inproceedings{henderson2014third,
  title={The third dialog state tracking challenge},
  author={Henderson, Matthew and Thomson, Blaise and Williams, Jason D},
  booktitle={2014 IEEE Spoken Language Technology Workshop (SLT)},
  pages={324--329},
  year={2014},
  organization={IEEE}
}

@article{williams2014dialog,
  title={The dialog state tracking challenge series},
  author={Williams, Jason D and Henderson, Matthew and Raux, Antoine and Thomson, Blaise and Black, Alan and Ramachandran, Deepak},
  journal={AI Magazine},
  volume={35},
  number={4},
  pages={121--124},
  year={2014}
}

@article{williams2016dialog,
  title={The dialog state tracking challenge series: A review},
  author={Williams, Jason and Raux, Antoine and Henderson, Matthew},
  journal={Dialogue \& Discourse},
  volume={7},
  number={3},
  pages={4--33},
  year={2016}
}

```
