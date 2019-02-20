# AV_Safety-Project

Artificial intelligence (AI)-driven technologies are being integrated into many activities that we take for granted. This project explores failures and disengagements in Autonomous Vehicles (AVs) being tested on public roads in California. The dataset you will be using however, while derived from the California Department of Motor Vehicles (DMV) database, has been sufficiently altered to be manageable for this project. As such, the results of the analysis you perform will not directly represent the California study. The analysis will use statistical and probabilistic approaches to evaluate how well the AI-driven decision and control of AVs works under a variety of conditions and developing insights into why/how they disengage.
Autonomous Vehicles are complex systems that use artificial intelligence (AI) and machine learning (ML) to integrate mechanical, electronic and computing technologies to make real-time driving decisions. 

Several states in the USA (e.g. California, Texas, Nevada, Pennsylvania, and Florida) and other parts of the world (e.g. China [1]) have already started field-testing AVs on public roads. As AVs have started interacting more directly with humans on public roads, the safety and resilience of AVs is a significant concern (Uber’s [2] fatal accident, Tesla’s [3] autopilot flaw) and must be thoroughly evaluated through analysis of data obtained during field-testing.
The California DMV mandates that all manufacturers testing AVs on public roads file annual reports detailing disengagements and accidents. A disengagement occurs when a failure in the AV system causes control of the vehicle to switch from software to the human driver.

In this project, you will study disengagement data from AV manufactures and analyze the current state of AV safety. The concepts you will learn and apply include the following
1. Handling datasets (Importing, extracting and summarizing features)
2. Basic statistical analysis of the dataset
3. Probabilistic Analysis of the data using concepts from ECE 313 (e.g., Probability, Conditional Probability, Bayes formula)
4. Create a Naive Bayes Machine Learning model to classify data based on features (e.g., weather conditions) in the dataset


**Dataset description:**
In a real-world setting, the data required for analysis might be spread across multiple sources. That is the case in our analysis too. Below is a description of the raw files in which the data is available and the data fields in the file. As mentioned previously, the data has been derived from California DMV, but has been sufficiently modified. Identicality to a known AV manufacturer is purely coincidental.

**mp1_av_disengagement.csv**
This file lists the details of each disengagement that happened in AV testing.
mp1_av_totalmiles.csv
This file contains the total number of miles driven and other summary statistics by month.

Month: Month and year when the disengagement happened

Car: ID of the AV

Location: Where the car was when the disengagement happened

Weather: Weather conditions when the disengagement happened
TypeOfTrigger: Whether the disengagement was automatic (decision taken by AV) or manual (decision taken by human driver)
ReactionTime: Time taken, in seconds, by the human driver to take control of the car after an automatic trigger.
NOTE: ReactionTime is not given for manual disengagements since it does not involve a trigger by the AV.
Cause: Reason for the disengagement

**mp1_av_totalmiles.csv**
Month: Month and year of AV testing
Car: ID of the AV
Miles driven: Total number of miles driven by the AV during the given month
Total number of disengagements: Number of disengagements during the given month
Number of automatic disengagements: Number of disengagements where the AV decided to give control to the human driver
Number of manual disengagements: Number of times the human driver decided to take control of the
