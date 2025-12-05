# Understanding Consumer Perception of Dot & Key Moisturizers: A Comparative NLP-Driven Review Analysis

**Owner:** Divya Bothra | **Capstone:** IIM Jammu, Social Media Analytics

---

## 🎯 Executive Summary

NLP-driven comparative analysis of **3,595 Flipkart reviews** across 4 Dot & Key moisturizer variants. Combines web scraping, preprocessing, NER/POS tagging, sentiment analysis, and topic modeling to generate **actionable product & marketing insights**.

**Finding:** 80% positive sentiment overall; hydrating gels (Blue) significantly outperform ceramide creams (Pink) due to better formulation-skin type fit.

---

## 📊 Dataset Overview

| Variant | Product | Reviews | Key Focus |
|---------|---------|---------|-----------|
| Orange | Vitamin C + E Sorbet Brightener | 479 | Brightening |
| Green | CICA Night Gel (Acne) | 868 | Sensitivity |
| Blue | 72hr Hydrating Gel + Probiotics | 1,307 | Hydration |
| Pink | Retinol + Ceramide Night Cream | 405 | Anti-Aging |

**Total:** 3,595 reviews (after deduplication)

---

## 🔧 Technical Pipeline

### 1. **Web Scraping**
- BeautifulSoup + Requests
- Multi-sort scraping (4 sort orders)
- Duplicate detection via fingerprinting

### 2. **Preprocessing**
- spaCy lemmatization & tokenization
- Regex cleaning (special chars, emojis)
- Stopword removal
- Output: `cleaned_reviews.xlsx`

### 3. **Linguistic Analysis**
- POS tagging: NOUN, ADJ, VERB extraction
- NER: Skin concerns (acne, oily), ingredients (ceramide, niacinamide)
- Frequency analysis & visualization

### 4. **Feature Engineering**
- **Bag-of-Words:** Top 50 terms per corpus
- **TF-IDF:** Variant-specific vocabulary extraction
- **Word2Vec:** 100-D embeddings, semantic clustering

### 5. **Sentiment Analysis**
- **VADER:** Lexicon-based (fast, interpretable)
- **ML Model:** TF-IDF + Logistic Regression
  - Accuracy: **80.48%** | F1-Score (Positive): **0.89**

### 6. **Topic Modeling**
- LDA (Latent Dirichlet Allocation)
- 4 overall topics | 2 topics per variant
- Output: `topic_summary_by_moisturizer.xlsx`

---

## 📈 Key Results

### Sentiment Distribution
- **Blue:** 85% positive (highest)
- **Green:** 82% positive
- **Pink:** 76% positive
- **Orange:** 74% positive

### Top Insights
- **Top Words:** good (1,380), product (1,199), skin (1,011), nice (542)
- **Top Adjectives:** lightweight, hydrating, gentle, non-greasy
- **Common Entities:** acne, oily skin, ceramide, hyaluronic acid

### ML Model Performance
| Metric | Score |
|--------|-------|
| Accuracy | 80.48% |
| Precision (Positive) | 0.82 |
| Recall (Positive) | 0.99 |
| F1-Score (Positive) | 0.89 |

---

## 💡 Key Recommendations

### Product Development
1. **Orange:** Launch fragrance-free variant (top complaint)
2. **Pink:** Create lightweight version for combination skin
3. **Green:** Develop day-use gel for broader appeal
4. **Blue:** Maintain current formulation (highest satisfaction)

### Marketing Strategy
1. **Segment-specific messaging:**
   - Blue → Oily/humid climate users
   - Pink → Dry/anti-aging segment
   - Green → Acne-prone/sensitive skin
   - Orange → Brightening/radiance seekers

2. **Hero Ingredient Marketing:** Emphasize ceramide, hyaluronic acid, niacinamide benefits

3. **Address Pain Points:** Highlight non-comedogenic, fragrance-free, lightweight properties in copy

---

## 📚 Technologies Used

| Category | Tools |
|----------|-------|
| **Language** | Python 3.8+ |
| **Data Collection** | BeautifulSoup, Requests |
| **NLP** | spaCy, NLTK, Gensim |
| **ML** | scikit-learn |
| **Visualization** | Matplotlib, Seaborn, WordCloud |
| **Data Processing** | Pandas, NumPy, openpyxl |

---

## 📄 License

Educational project for IIM Jammu MBA program.

---

## 📞 Questions?

Reach out via GitHub Issues or contact the team directly @mba24077@iimj.ac.in



