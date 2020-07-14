# PepGAN

PepGAN is a generative adversarial network for peptide sequence generation which incorporates knowledge about negative samples via classifier network (activity predictor).

Details about PepGAN methodology can be found here

https://chemrxiv.org/articles/Generating_Ampicillin-Level_Antimicrobial_Peptides_with_Activity-Aware_Generative_Adversarial_Networks/12116136

PepGAN employs part of the benchmarking platform Texygen for more details see

https://github.com/geek-ai/Texygen

# To Run

* To use PepGAN for antimicrobial peptide (AMP) generation use following command:

  python main.py -g pepgan -t real -d data/output_amp.txt

* To run PepGAN on own sequences you have to train activity predictor first using own data via following command:

  python classifiertrain.py

  Afterwards link to the trained model should be added into the PepganReward.py file <br /><br />

