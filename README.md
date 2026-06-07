#  EX-02: Cross-Platform Prompting – Evaluating Diverse Techniques in AI-Powered Sentiment Analysis

##  AIM

To evaluate and compare the effectiveness of different prompting techniques (Zero-shot, Few-shot, Chain-of-Thought, and Role-based Prompting) across multiple AI platforms for performing sentiment analysis on social media content.

---

#  Scenario

You are working as a data analyst for a digital marketing company. The company wants to understand customer opinions about a newly launched smartphone by analyzing social media reviews.

Your task is to use different AI platforms and prompting strategies to classify customer feedback into **Positive**, **Negative**, or **Neutral** sentiments and determine which approach provides the most reliable results.

### Evaluation Metrics

* Accuracy
* Consistency
* Interpretability
* Speed
* User Experience

---

#  Algorithm

## Step 1: Dataset Selection

Select customer reviews related to a smartphone launch.

### Sample Reviews

**Review 1**

> "The camera quality is excellent and battery backup lasts all day."

**Review 2**

> "The phone overheats frequently during gaming sessions."

**Review 3**

> "The design looks premium but the software needs improvement."

**Review 4**

> "Excellent performance and smooth user experience."

**Review 5**

> "The charging speed is slow compared to competitors."

---

## Step 2: Prompting Strategies Definition

### Zero-Shot Prompting

Ask the AI directly to identify sentiment without providing examples.

"Classify the sentiment of the following reviews as Positive, Negative, or Neutral."

### Few-Shot Prompting

Provide 2–3 sentiment classification examples before asking the AI to classify reviews.

"Prompt with Examples:

Example 1:
Review: "Amazing battery life and fast charging."
Sentiment: Positive

Example 2:
Review: "The device crashes frequently and feels sluggish."
Sentiment: Negative

Example 3:
Review: "Good display quality but average speakers."
Sentiment: Neutral

Now classify the following reviews:"

### Chain-of-Thought Prompting

Request the AI to explain reasoning before providing the final classification.

"Analyze each review, explain the reasoning, and then provide the sentiment classification."

### Role-Based Prompting

Ask the AI to act as a market research analyst and evaluate customer sentiment.

"Act as a Market Research Analyst. Evaluate customer feedback and identify the sentiment expressed in each review."

---

## Step 3: Platform Selection

The following AI platforms are used:

* ChatGPT (OpenAI)
* Gemini (Google)
* Claude (Anthropic)
* Copilot (Microsoft)

---

## Step 4: Execution

For each platform:

1. Apply all prompting strategies.
2. Record sentiment predictions.
3. Measure response generation time.

---

## Step 5: Evaluation Criteria

Evaluate based on:

* Accuracy
* Consistency
* Interpretability
* Speed
* User Experience

---

## Step 6: Scoring and Analysis

1. Assign scores from 1–5.
2. Compare outputs.
3. Identify the best-performing combination.

---

#  Output

## ChatGPT

### Zero-Shot

```text
Review 1 – Positive
Review 2 – Negative
Review 3 – Neutral
Review 4 – Positive
Review 5 – Negative
```

### Few-Shot

```text
Positive:
"The battery life is amazing."

Negative:
"The device lags often."

Classification Results:

Review 1 – Positive
Review 2 – Negative
Review 3 – Neutral
Review 4 – Positive
Review 5 – Negative
```

### Chain-of-Thought

```text
Review 1 mentions strong camera quality and battery performance, indicating satisfaction.

Review 2 highlights overheating issues, indicating dissatisfaction.

Review 3 contains both positive and negative opinions, making it Neutral.

Review 4 expresses clear satisfaction with performance.

Review 5 complains about charging speed.

Final Classification:

Positive – Reviews 1 and 4
Neutral – Review 3
Negative – Reviews 2 and 5
```

### Role-Based

```text
As a market research analyst, I conclude that customers appreciate the phone's camera quality and performance. However, concerns regarding overheating and charging speed negatively impact overall satisfaction.

Sentiment Summary:

Positive – 40%
Neutral – 20%
Negative – 40%
```

---

## Gemini

### Zero-Shot

```text
Positive:
Reviews 1 and 4

Negative:
Reviews 2 and 5

Neutral:
Review 3
```

### Few-Shot

```text
Example:
"The screen quality is excellent." → Positive

"The battery drains quickly." → Negative

Results:

Review 1 – Positive
Review 2 – Negative
Review 3 – Neutral
Review 4 – Positive
Review 5 – Negative
```

---

## Claude

### Chain-of-Thought

```text
The reviews indicate mixed customer opinions.

Strengths:
- Camera quality
- Performance
- Battery life

Weaknesses:
- Heating issues
- Slow charging

Classification:
Positive – Reviews 1 and 4
Neutral – Review 3
Negative – Reviews 2 and 5
```

### Role-Based

```text
As a consumer insights expert, I observe that customers generally appreciate hardware performance and design quality. However, thermal management and charging efficiency remain areas requiring improvement.

Overall Sentiment:
Positive Dominance with notable negative concerns.
```

---

# 📈 Performance Comparison

| Platform | Prompt Type      | Accuracy | Consistency | Interpretability | Speed | UX | Total (/25) |
| -------- | ---------------- | -------- | ----------- | ---------------- | ----- | -- | ----------- |
| ChatGPT  | Zero-shot        | 4        | 4           | 4                | 5     | 5  | 22          |
| ChatGPT  | Few-shot         | 5        | 5           | 5                | 4     | 5  | 24          |
| ChatGPT  | Chain-of-Thought | 5        | 5           | 5                | 4     | 5  | 24          |
| ChatGPT  | Role-based       | 5        | 5           | 5                | 4     | 5  | 24          |
| Gemini   | Zero-shot        | 4        | 4           | 4                | 5     | 4  | 21          |
| Gemini   | Few-shot         | 4        | 5           | 4                | 4     | 4  | 21          |
| Claude   | Chain-of-Thought | 5        | 5           | 5                | 4     | 5  | 24          |
| Claude   | Role-based       | 5        | 5           | 5                | 4     | 5  | 24          |

---

# ✅ Result

The analysis shows that **ChatGPT** and **Claude** provide the most accurate and interpretable sentiment analysis results.

### Key Findings

* Chain-of-Thought prompting improves reasoning and explainability.
* Role-based prompting improves contextual understanding.
* Few-shot prompting increases consistency.
* Zero-shot prompting offers the fastest response generation.

### Best Performing Techniques

🥇 Chain-of-Thought Prompting

🥇 Role-Based Prompting

These techniques achieved the highest overall scores for sentiment classification tasks.

---

# 📚 Conclusion

This experiment demonstrates that prompt engineering significantly influences AI performance in sentiment analysis.

Among the evaluated approaches:

* Chain-of-Thought Prompting provided the most transparent reasoning.
* Role-Based Prompting produced domain-aware insights.
* Few-Shot Prompting improved classification consistency.
* Zero-Shot Prompting delivered faster responses with acceptable accuracy.

Therefore, selecting the appropriate prompting strategy is essential for obtaining reliable sentiment analysis results from modern AI systems.
