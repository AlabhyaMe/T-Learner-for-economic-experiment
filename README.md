# Meta Learners for Policy Intervention

This repository contains the implementation of RCT-based causal inference and Meta Learners (T-Learners) to optimize policy interventions by targeting individuals who are most likely to benefit.

Project Overview
    
    The project explores different methods for estimating treatment effects and scaling up an intervention program efficiently. It includes-
    
    Randomized Controlled Trials (RCT): The baseline experiment to estimate the impact of treatment.
    
    Linear Regression: A simple method to identify key predictors of expenditure.
    
    T-Learners: A causal machine learning approach that builds separate models for treated and control groups to estimate individualized treatment effects.
    
    T-Learners allow for better targeting in policy interventions by identifying individuals who would benefit the most, making policy implementation more effective and equitable compared to random assignment.

Files and Structure

1. Meta_Learners.ipynb

   This is the main notebook containing the code and workflow for

    Analyzing the RCT dataset
    
    Running linear regression to identify key variables affecting expenditure
    
    Implementing T-Learners to estimate individual treatment effects
    
    Scaling up the program using a dataset of 1 million people

3. dataset.csv

   This is the primary dataset, which contains information from the RCT experiment. It is used for training models, evaluating treatment effects, and building the T-Learner model.

4. new_target.csv

   A scaled-up dataset representing a 1 million-person population, used to simulate a large-scale intervention. The T-Learner model is applied here to target 200,000 individuals most likely to benefit from treatment.

5. data_processor.ipynb

   This notebook processes the output from Meta_Learners and simulates the impact of treatment. It helps estimate the overall effect on expenditure when selecting individuals based on random assignment vs. T-Learner targeting.

Key Insights
    
    Random assignment is fair but may not maximize impact.

    T-Learners allow targeted interventions, improving efficiency by selecting those most likely to benefit.

    Scaling up policies with data-driven targeting can optimize resource allocation while ensuring equity.

How to Use
    
    Run Meta_Learners.ipynb to process the RCT dataset and build models.

    Use data_processor.ipynb to simulate the impact of treatment on a larger population.

Compare different approaches (random vs. targeted assignment) to understand their effects.

Applications
    
    This approach can be applied to various policy interventions, such as:
    
    Healthcare subsidies (targeting individuals who benefit most)
    
    Education grants (selecting students with the highest projected impact)
    
    Welfare programs (optimizing government spending for maximum social benefit)
