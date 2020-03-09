# Modeling-Precision-Medicine
In this project we discuss biomedical applications of clustering methods and integration of multi-omics data. Specifically, we show that unsupervised machine learning methods can identify distinct subtypes in a set of samples associated with the same pathology. We also touch on questions related to classification and feature selection.

Key Concepts:

Molecular Profiling: Gene panels used to determine cancer subtype, such as PAM50 that is used to determine breast cancer subtypes from gene expression data. This profiling sometimes relies on genomics data (mutations) and sometimes on transcriptomics data (gene/isoform expression). This project will look at those types of features as well as combinations of features that have more predictive power for therapeutic efficacy.

Precision Medicine: Precision Medicine is an emerging approach for disease treatment and prevention that takes into account individual variability in genes, environment, and lifestyle for each person

Predicting Therapeutic Response: A major limitation of precision medicine is it’s limiting factor of more traditional therapeutics that are designed to work for anyone with a broad disease definition. Therefore, precise identification of patients that will respond to a therapeutic has been a major challenge in the clinical trials that are a major step in getting a therapeutic into clinical use. Methods of predicting response are critical for getting more precision therapeutics to patients.

Levels of molecular regulation: Multiomics means a new biological analyses approach where the data sets are multiple omes such as genome, proteome, transcriptome, epigenome, and microbiome. By combining these “-omes” into a set of “-omes”, one can analyze the complex big data efficiently enough to find biomarkers easily.

Machine Learning for Biomedical Data: Machine learning today was born from pattern recognition and the theory that computers can learn without being programmed to perform specific tasks. The iterative aspect of machine learning is important because as models are exposed to new data, they are able to independently adapt. They learn from previous computations to produce reliable, repeatable decisions and results.

 

Practical Skills:

Missing Data Approximation: Our drug-efficacy table contains missing values (missing values are shown as “NA”, which stands for “not available”). But the majority of analysis methods can’t cope with missing values. We will learn how to use specialized methods to fill in missing values for further analysis. In order to “restore” a value for a sample (cell line) C and feature (drug) D based on available values we can find samples similar to C and “transfer” values from that samples associated with D to the table cell being filled. Alternatively, we can find features similar to D and “transfer” values from that features associated with the sample C.

Classification: This project includes multiple cancer subtypes (luminal, basal, claudin-low and normal-like). Can we identify the subtype for a given sample based on gene expression and can we find genes that are the most informative for this identification. Answers to these questions are provided by supervised machine learning methods, specifically, classification algorithms.

Feature Selection: Using Stepwise LDA to select most informative features for classification: Stepwise feature selection starts with testing all individual features and selects the one that provides the best classification quality (for the training set). Than it tests all pairs where the first feature is the one selected at the previous step, and again it selects the pair that provides the best classification quality. The process goes further to triples, quadruples, etc. Such greedy strategy is not generally optimal, but it provides the result in an acceptable time.

Clustering: classification methods can provide reliable identification of a class (e.g., pathology subtype) for a sample. This identification can be clinically important: for example, it can be used for optimal selection of therapy scheme. But methods for classification are supervised: they need a training set with initially known separation into classes. If we don’t have an annotated dataset, we need to learn to use clustering methods. These are aimed at division of the set of samples into subgroups – clusters – in such a way that similar samples are grouped together in one cluster, while dissimilar samples are attributed to different clusters.

Multi-Omics Integration: One application of multi-omics data is to identify molecular signatures that can be used to assign specific treatment to individual patients. However, strategies to develop optimal predictive marker sets are still being explored. Indeed, it is not yet clear which molecular data types (genome, transcriptome, proteome, and so on) will be most useful as response predictors. Here we evaluate various data types and an integration model to assign treatments and select similar molecules that can be potentially used for similar efficacy.
