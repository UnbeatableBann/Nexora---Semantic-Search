# Vibe Matcher

A simple AI-powered fashion recommender that matches product vibes to a user’s mood or query. It uses text embeddings and cosine similarity to find the top 3 products that best match the input vibe.

## Features

* Sample fashion dataset with product names and descriptions
* Text embeddings using Gemini API
* Cosine similarity matching
* Visualization of similarity scores with "good" matches labeled
* Latency tracking and basic evaluation metrics

## How It Works

1. The script loads mock fashion data into a Pandas DataFrame.
2. Product descriptions and a user vibe query are embedded using the Gemini Embedding model.
3. Cosine similarity is calculated between the query and all products.
4. The top 3 matching products are displayed with similarity scores and "good" tags for scores above 0.7.
5. Results are plotted for easy visualization.

## Setup

1. Clone the repository
2. Install dependencies

   ```bash
   pip install -r requirements.txt
   ```
3. Set up your Gemini API key

   ```bash
   export GEMINI_API_KEY="your_key_here"
   ```
4. Run the notebook or script

   ```bash
   python vibe_matcher.py
   ```

## Notes

This is a prototype built for testing the idea of vibe-based fashion recommendations. Future improvements could include larger datasets, Pinecone or FAISS integration, and web deployment.
