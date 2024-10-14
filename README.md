# Prompt Collection for LLM and Search Analysis

This repository contains a set of structured prompts designed for the annotation, summary, and analysis of search results using LLM (Large Language Models). The files aim to facilitate tasks such as political leaning, stance detection, subjectivity classification, bias measurement, sentiment analysis, and filter bubble investigation. Below is a description of each file and its purpose.

## Files Overview

1. **search_history_prompt.txt**  
   - **Description:**  
     This prompt defines guidelines for creating search history queries reflecting different user perspectives (supportive, neutral, opposing) for a given topic. The objective is to simulate diverse viewpoints to study search result behaviors.  
   - **Key Elements:**  
     - Definition of perspectives (Support, Neutral, Oppose)  
     - Examples for topics like *Climate Change* and *Healthcare Reform*  
     - Instructions for generating 50 search history terms per perspective

2. **llm_summary_prompt.txt**  
   - **Description:**  
     This prompt provides detailed instructions for summarizing LLM-analyzed search result datasets. It explains how to categorize and analyze user contexts and filter bubble tendencies based on search query results.  
   - **Key Elements:**  
     - User context instances (Geolocation, Language, Device Environment)  
     - Definition of analysis targets (Political, Stance, Sentiment, Subjectivity, Bias)  
     - Guidelines for conducting comparative analysis and deriving filter bubble implications  

3. **llm_annotation_role_prompt.txt**  
   - **Description:**  
     This prompt outlines the responsibilities of professional annotators who label articles based on criteria such as political leanings, sentiment, and subjectivity. It provides instructions for consistent and nuanced labeling using decimal scores to reflect intensity.  
   - **Key Elements:**  
     - Labeling guidelines for five criteria (Political, Stance, Sentiment, Subjectivity, Bias)  
     - Output in JSON format  
     - Example annotations for topics like *Biden*, *Trump*, and *Immigration*  

4. **llm_annotation_request_prompt.txt**  
   - **Description:**  
     This file serves as a template for structuring input and output during the annotation process. It ensures uniformity in annotation requests and responses by defining the input format (query, title, and context) and requiring JSON-based outputs.  
   - **Key Elements:**  
     - Input structure: `{query}`, `{title}`, `{detail_context}`  
     - Placeholder for JSON output with labels and scores  

## Usage

1. **Search History Simulation:**  
   Use `search_history_prompt.txt` to create hypothetical search queries reflecting multiple viewpoints on topics of interest. These can help study the influence of search engine algorithms on results based on user perspectives.

2. **LLM-Based Summary and Analysis:**  
   Utilize `llm_summary_prompt.txt` for summarizing datasets by categorizing user behaviors, analyzing political and sentiment-based trends, and investigating filter bubble formation.

3. **Annotation Tasks:**  
   - Refer to `llm_annotation_role_prompt.txt` to annotate news articles based on five analytical criteria with detailed scoring and labeling.
   - Use `llm_annotation_request_prompt.txt` as a template for structuring input and generating JSON-based annotation outputs.
