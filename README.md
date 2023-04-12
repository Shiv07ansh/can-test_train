# can-train-and-test

**This repository provides controller area network (CAN) datasets for the training and testing of machine learning schemes. The datasets are derived from the [can-dataset](https://bitbucket.org/brooke-lampe/can-dataset/src/master/) and [can-ml](https://bitbucket.org/brooke-lampe/can-ml/src/master/) repositories.**

This repository contains controller area network (CAN) traffic for the 2017 Subaru Forester, the 2016 Chevrolet Silverado, the 2011 Chevrolet Traverse, and the 2011 Chevrolet Impala.

For each vehicle, there are samples of attack-free traffic--that is, normal traffic--as well as samples of various types of attacks.

The samples are stored in comma-separated values (CSV) format. All of the samples are labeled; attack frames are assigned "1," while attack-free frames are designated "0."

This repository has been curated into four datasets, dubbed "set_01," "set_02," "set_03," and "set_04." For each dataset, there are five sub-datasets: one training sub-dataset and four testing sub-datasets. Each sub-dataset contains both attack-free and attack data.

### Sub-datasets:

*  **train_01:**  Train the model
*  **test_01_known_vehicle_known_attack:**  Test the model against a known vehicle (seen in training) and known attacks (seen in training)
*  **test_02_unknown_vehicle_known_attack:**  Test the model against an unknown vehicle (not seen in training) and known attacks (seen in training)
*  **test_03_known_vehicle_unknown_attack:**  Test the model against a known vehicle (seen in training) and unknown attacks (not seen in training)
*  **test_04_unknown_vehicle_unknown_attack:**  Test the model against an unknown vehicle (not seen in training) and unknown attacks (not seen in training)
