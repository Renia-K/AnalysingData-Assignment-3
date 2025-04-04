# AnalysingData-Assignment-3

Probing Large Language Models & Genre Classification

## Overview

This project aims to:

1.   Investigate whether an LLM’s internal representation of a story is closer to the book version or the movie version through probing. This includes a research outline, a mini experiment with an open-source LLM, and a discussion of results.

2.   Using Python's Ollama library, classify song lyrics by genre using two prompting strategies—Zero-shot and Few-shot. The model’s performance is evaluated using Precision, Recall, and F1 score. Also a discussion of the results is included.

***For both parts the discussion is submitted via Brightspace and not directly in the repository.


# PART 1: Research Project: Investigating Large Language Models' Internal Representations of Twilight

## Overview
This repository contains the research and analysis of how OpenAI’s ChatGPT-3.5, encode narratives from the Twilight book (2005) and its movie adaptation "Twilight" (2008). The project investigates whether LLMs lean more towards the textual descriptions of the book or the visual and script-based narrative of the movie when responding to factual questions about selected common scenes. 


# Methodology
The experiment involves:

1. Key scene extraction from both movie and book. 

2. Design of neutral, factual questions about the scenes to test the LLM's alignment.

3. Running the questions in two formats:

`First method`: Asking the questions without providing passages to the model.

`Second method`: Providing the model with text excerpts from both the book and movie before asking questions.


# The responses are analyzed and categorized into:

1. Book-aligned (matching the book)

2. Movie-aligned (matching the movie)

3. Both (containing elements of both)

4. Inaccurate (incorrect or AI-generated fiction)

   
# Results

1. Using the first method, 12.5% of answers aligned with the book, 25% with the movie, and 31.25% had elements of both.

2. Using the second method, 31.25% of answers aligned with the book, 12.5% with the movie, and 43.75% contained a mix of both.

3. The rest of the answers in both methods were inaccurate, demonstrating gaps in the model’s ability to consistently replicate the narrative.

# Tools & Resources
Model: OpenAI ChatGPT-3.5

Data: Extracted passages from the Twilight book and movie script from Project Gutenberg & The Internet Movie Script Database (IMSDb)

Supporting Tools: Python for text cleaning and normalization

# Files

`Assignment3_Part1`: python notebook for text cleaning and normalization
`twilight`: extracted passages in preliminary format 
`twilight_data_cleaned`: CSV. file output from Python notebook

# NOTE
Both report with results as well as the prompts used and the answers are included in the files: Part1_Prompts & Report_Assignment3_KormaTS_S6006965


# PART 2: Annotation of songs’ lyrics using Ollama

## Overview

This project includes the annotation of song lyrics' genres with the Llama3 model from Ollama's Python library. The model is demonstrated in both Zero-Shot and Few-Shot prompting approaches in classifying song lyrics into different genres, including Rock, Electronic, Hip-Hop, Pop, and others.

The annotated genres are: Rock, Electronic, Hip-Hop, Pop, Other, R&B, Country, Jazz, Metal, Folk and Indie.

## Model Selection

The Llama3 model was chosen over Mistral since it has a superior natural language understanding and also has multilingual capabilities. This becomes especially important for the analysis of song lyrics in different languages since Llama3 is more capable of handling multilingual input than Mistral.

## Prompting Strategies

`Zero-Shot Prompting`
`Few-Shot Prompting`

**Zero-Shot Classification Report**

**Accuracy**: 0.00  
**Macro Avg**: Precision 0.00, Recall 0.00, F1-Score 0.00  
**Weighted Avg**: Precision 0.00, Recall 0.00, F1-Score 0.00

| Category   | Precision | Recall | F1-Score |
|------------|-----------|--------|----------|
| Classical  | 0.00      | 0.00   | 0.00     |
| Country    | 0.00      | 0.00   | 0.00     |
| Electronic | 0.00      | 0.00   | 0.00     |
| Folk       | 0.00      | 0.00   | 0.00     |
| Hip-Hop    | 0.00      | 0.00   | 0.00     |
| Indie      | 0.00      | 0.00   | 0.00     |
| J-Pop      | 0.00      | 0.00   | 0.00     |
| Jazz       | 0.00      | 0.00   | 0.00     |
| Metal      | 0.00      | 0.00   | 0.00     |
| Non        | 0.00      | 0.00   | 0.00     |
| Other      | 0.00      | 0.00   | 0.00     |
| Pop        | 0.00      | 0.00   | 0.00     |
| R&B        | 0.00      | 0.00   | 0.00     |
| Rap        | 0.00      | 0.00   | 0.00     |
| Rock       | 0.00      | 0.00   | 0.00     |
| unknown    | 0.00      | 0.00   | 0.00     |


**Few-Shot Classification Report**

**Accuracy**: 0.07  
**Macro Avg**: Precision 0.01, Recall 0.06, F1-Score 0.01  
**Weighted Avg**: Precision 0.01, Recall 0.07, F1-Score 0.01

| Category   | Precision | Recall | F1-Score |
|------------|-----------|--------|----------|
| Classical  | 0.00      | 0.00   | 0.00     |
| Country    | 0.00      | 0.00   | 0.00     |
| Electronic | 0.00      | 0.00   | 0.00     |
| Folk       | 0.00      | 0.00   | 0.00     |
| Hip-Hop    | 0.00      | 0.00   | 0.00     |
| Indie      | 0.00      | 0.00   | 0.00     |
| J-Pop      | 0.00      | 0.00   | 0.00     |
| Jazz       | 0.00      | 0.00   | 0.00     |
| Metal      | 0.00      | 0.00   | 0.00     |
| Non        | 0.00      | 0.00   | 0.00     |
| Other      | 0.00      | 0.00   | 0.00     |
| Pop        | 0.00      | 0.00   | 0.00     |
| R&B        | 0.00      | 0.00   | 0.00     |
| Rap        | 0.00      | 0.00   | 0.00     |
| Rock       | 0.09      | 1.00   | 0.17     |
| unknown    | 0.00      | 0.00   | 0.00     |


## NOTE
Report with results and suggestions for improvement is submitted under the file name Report_Assignment3_KormaTS_S6006965.



## Creator
This dataset was created and curated by Theodora-Stavroula Korma on behalf of the course Analysing Data, for the MA Digital Humanities.

Contact Information: email: t.s.korma@student.rug.nl
