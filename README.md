# Continuous user authentication in web applications through behavioral biometrics

This is the code I used and the service I created for the purpose of my under-graduate thesis in the Department of Electrical and Computer Engineering in Aristotle University of Thessaloniki.

PM me if you'd like to experiment with the dataset of keystrokes collected from real users, or if you'd like to read the whole thesis report (... in greek :)). 

## Repo Structure

* **continuous-authentication-service**: This is the main service created, which provides a continuous authentication system using keystroke dynamics in order to authenticate users with their typing pattern.
* **continuous-authentication-website**: In order to collect keystrokes from real users and to apply this authentication system on them, a website was created which provides various user scenarios where a user is required to type something.
* **continuous-authentication-experiments**: This is the final chapter of this work. It includes pattern recognition techniques in order to measure the performance (FAR, FRR, EER etc) of the system. Such techniques are Anomaly/Outlier/Novelty detection, Classification with 1vs1 reduction & majority vote etc. 

## Thesis Abstract

The use of continuous authentication systems that employ behavioral biometrics are gradually gaining ground as the preferred method of authentication. This is due to the limitations imposed by standard authentication methods, which are unable to guarantee user identity beyond initial authentication and conceal serious security issues such as impersonation and exposure of personal data to third parties. On the other hand, a user's behavioral biometric trait is very difficult to be copied or intercepted in any way, and as a result it can be used appropriately for the implementation of a continuous authentication system, ensuring this way a secure session for the user.  
Within the context of this thesis we choose as a behavioral biometric trait the way a user interacts with his/her keyboard. Practically, we use keystroke dynamics to identify and authenticate users. Specifically, we analyze the keystroke digraphs of a user that are collected from the typing of words, and extract three features: hold time of the first key of a digraph, hold time of the second key and time elapsed since the release of the first key and the presssing of the second key.  
In order to test and evaluate the implemented system we collected a total of 59000 keystroke events, from 37 subjects within a period of 12 weeks. Using that data, we tested various pattern recognition models such as classification and outlier detection, while experimenting at the same time with data pre-processing techniques for the reduction of feature vector dimensions (PCA). The best results are obtained by employing an One-Class SVM for a 3-d feature vector, achieving 0.61% False Accept Rate (FAR) and 0.75% False Reject Rate (FRR), and by employing Gaussian Mixture Models for a 2-d feature vector, this way achieving 1.35% FAR and 1.71% FRR.  
Our results show that keystroke dynamics can be used effectively in a continuous authentication system.

Anastasios Kakouris  
**tasoskakour@gmail.com**  
*February 2018, Thessaloniki Greece*
