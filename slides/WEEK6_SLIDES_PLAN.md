# Week 6: Ensemble Methods & Stacking - Slide Plan

## Overview
- **Format**: LaTeX Beamer (consistent with Week 4 & 5)
- **Aspect Ratio**: 16:9
- **Theme**: Madrid (consistent with existing slides)
- **Total Slides**: ~35-40
- **Approximate Duration**: 45-50 minutes

---

## Slide Structure

### Section 1: Title & Outline (Slides 1-2)
**Slide 1: Title Page**
- Title: "Week 6: Ensemble Methods & Stacking"
- Subtitle: "Heart Failure Survival Analysis"
- Date: Winter 2026

**Slide 2: Outline / Table of Contents**
- Week 5 Recap
- Why Ensemble Methods?
- Voting Classifier
- Bagging
- Boosting (Gradient Boosting & LightGBM)
- Stacking
- Performance Comparison
- Kaggle Challenge

---

## Key Sections

### Section 2: Week 5 Recap (Slides 3-4)
- Quick recap of hyperparameter optimization
- Baseline RF performance: 73% accuracy
- Motivation: Can we combine models for better results?

### Section 3: Why Ensemble Methods? (Slides 5-7)
- Bias-variance trade-off review
- When ensembles work: Diversity, Accuracy, Independence
- Types: Parallel (Voting, Bagging) vs Sequential (Boosting) vs Stacking

### Section 4: Voting Classifier (Slides 8-11)
- Panel of doctors analogy
- Hard voting (majority rule) vs Soft voting (average probability)
- Base learners: RF + LR + SVM (diverse!)
- Results comparison

### Section 5: Bagging (Slides 12-15)
- Bootstrap sampling concept
- Out-of-Bag (OOB) score as free validation
- Why bagging reduces variance
- Bagging vs Random Forest distinction

### Section 6: Boosting (Slides 16-20)
- Sequential learning philosophy: "Learn from mistakes"
- Bagging vs Boosting comparison table
- Gradient Boosting concepts and key parameters
- Staged learning curves (F1 vs n_estimators)

### Section 7: LightGBM (Slides 21-24)
- Why LightGBM: Leaf-wise growth, speed, efficiency
- Key parameters: num_leaves, learning_rate, max_depth
- Optuna for hyperparameter tuning (50 trials, log-scale learning_rate)
- Week 6 Results: LightGBM Tuned achieves +17.4% improvement on MCC

### Section 8: Stacking (Slides 25-29)
- Level 0 (base learners) & Level 1 (meta-learner) architecture
- **Data Leakage Warning**: Out-of-fold predictions (critical!)
- How to implement stacking properly
- Meta-learner coefficients: Which base learner trusted most?

### Section 9: Comparative Analysis (Slides 30-32)
- Heatmap: All 8 models × 4 metrics
- Grouped bar charts with baseline reference line
- When to use each ensemble method

### Section 10: Connection to Paper & Practice (Slides 33-34)
- Chicco & Jurman 2020: MCC is best for imbalanced data
- Our validation: MCC +17.4% improvement proves paper's recommendations
- Key takeaways: Single models have limits, ensembles help, small data = limited gains

### Section 11: Kaggle Challenge (Slide 35)
- Objective: Beat Stacking MCC baseline (~0.45)
- Rules: random_state=21, test_size=0.3, max 100 Optuna trials
- Hints: ExtraTreesClassifier, passthrough=True, different voting strategies

### Section 12: Closing (Slide 36)
- Summary of ensemble methods
- Key metrics: Report all 4 (Accuracy, F1, ROC-AUC, MCC)
- Resources for learning (StatQuest, LightGBM docs)

---

## Design & Timing

### Visual Consistency
- Madrid theme (light background, dark text)
- Monospace for code snippets
- Tables for hyperparameter comparisons
- Line plots for learning curves
- RdYlGn heatmaps

### Presentation Timing (50 min)
- Title & Outline: 2 min
- Recap & Motivation: 4 min
- Why Ensembles: 3 min
- Voting: 5 min
- Bagging: 5 min
- Boosting: 8 min
- LightGBM: 6 min
- Stacking: 8 min
- Comparison: 5 min
- Paper Connection & Challenge: 3 min
- Q&A: 2 min

### Interactive Elements
- Ask: "Why did soft voting work better?"
- Discuss: "Why do different metrics show different winners?"
- Leaderboard: Present Kaggle challenge results
- Q&A: "Why is data leakage bad?"

---

## Expected Slides: ~36 total
- 12 sections
- Mix of concept slides, results slides, comparison slides
- Consistent with Week 4 & 5 presentations

## Next Step
Create `week6_slides.tex` using LaTeX/Beamer format following this plan.
