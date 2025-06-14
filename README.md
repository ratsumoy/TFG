# EXPLORING HATE SPEECH IN POLITICAL CONTENT ON TIKTOK

**BACHELOR’S FINAL THESIS OF**
Montserrat Sumoy Solé
**Supervisor:** Diego Saez

---

## Abstract

This study investigates the political sentiment and user reactions on TikTok during Spain’s 2023 general elections. By analysing videos and comments from official accounts of parties represented in the Spanish Congress, the research applies a sentiment and hate-speech detection model – RoBERTuito – to assess the discourse on the platform. Results indicate that far right and left-wing parties, such as Vox and Podemos, tend to publish content with higher levels of negativity. While right-wing content often receives stronger user support, despite its polarizing discourse, the study reveals that left-wing parties receive more critical or sarcastic comments, and that hate speech appears more frequently. Additionally, the findings highlight the limitations of current NLP models in capturing sarcasm, irony and multilingual content on TikTok. This research contributes to the understanding of digital political discourse and underscores TikTok’s unique role in shaping youth political engagement.

---

## Code

The code is divided into two main parts: one for video analysis and one for comment analysis.

### 1. Video Analysis

This part focuses on extracting and processing video metadata, including descriptions and transcriptions. It uses a CSV file as input, generated via the TikTok API (`getVideoData`). The code then applies sentiment and hate speech models to the text.

### 2. Comment Analysis

This part processes the comments associated with the selected videos. After extracting comment data using the same API (`getCommentsData`), it computes sentiment and hate speech metrics using RoBERTuito. It also includes scripts for manual annotation, allowing comparison between model predictions and human-labelled categories such as Supportive, Sarcastic, Hate, Negative, and Other (Case Study)
