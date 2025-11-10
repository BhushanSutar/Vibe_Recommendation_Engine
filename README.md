# Nexora Vibe Matcher

A vibe-driven fashion recommendation system that matches user mood and style intent to clothing items. Instead of searching by keywords, the system understands aesthetic cues like “minimal”, “urban streetwear”, or “neutral relaxed fit” and recommends products that feel aligned with that vibe.

---

##  Project Summary

The goal of this project is to create a *vibe-aware recommendation engine* that returns fashion products based on the **aesthetic intention** expressed by the user. This is done using:

- Local semantic embeddings (all-MiniLM-L6-v2)
- Cosine similarity for matching
- Rule-based vibe tagging for style context
- A hybrid scoring model for personalization

This aligns with Nexora.fashion’s mission of creating **vibe-first discovery** experiences for Gen Z and millennial fashion culture.

---

##  Key Features

- **No API Key Needed:** Uses a local sentence transformer model because OpenAI free credits expired — resulting in an **offline, stable, cost-free** pipeline.
- **Cosine Similarity Matching:** Finds semantically relevant clothing items.
- **Vibe Tagging Layer:** Captures aesthetic style attributes like `minimal`, `neutral`, `utility`, `relaxed`, `dark`.
- **Hybrid Scoring System:**  
  `final_score = 0.7 * semantic_similarity + 0.3 * vibe_alignment_score`
- **Fallback Threshold:** Avoids poor matches by rejecting low-confidence results.
- **Latency Evaluation:** Measures performance for real product usability.

---

##  Stack Used

- Python
- Pandas / NumPy
- scikit-learn
- SentenceTransformers (`all-MiniLM-L6-v2`)
- Matplotlib (for latency visualization)

---

