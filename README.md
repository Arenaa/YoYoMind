# YoYoMind

A Computational Model of Self-Belief Dynamics in Borderline Personality Disorder (BPD)

YoYoMind is a framework designed to quantify and analyze the dynamics of self-belief in individuals with Borderline Personality Disorder using language-based signals. By leveraging transformer-based NLP models, YoYoMind computes interpretable metrics across thousands of social media posts to reveal patterns of emotional instability, contradiction, sentiment, and identity disturbance. 


 Repository Structure

1- YoYoMind.ipynb
    Core Scoring Pipeline
    This notebook computes four fundamental linguistic metrics at both the sentence and user level:

    Emotion
    Sentiment
    Contradiction
    Dominant theme

2- Analysis1.ipynb
    Dimensionality Reduction & Exploratory Analysis
    Visualizes feature distributions via histograms
    Applies Principal Component Analysis (PCA) to reveal latent structureUses Linear Discriminant Analysis (LDA) to assess group separability between BPD and control users

3- Analysis2.ipynb
    Emotion Dynamics & Group Comparison
    Visualizes temporal emotion shifts at the user level using line plots and heatmaps
    Summarizes group-level trends in a comparison table, highlighting contrasts in linguistic behavior between BPD and control groups

4- Control_group_Data_Preparation.ipynb
    Control Group Construction
    Retrieves Reddit user data using the PRAW API
    Filters out users with any history in mental health-related subreddits (e.g., r/BPD)
    Selects high-activity users (100+ posts) to ensure a robust and unbiased control sample
