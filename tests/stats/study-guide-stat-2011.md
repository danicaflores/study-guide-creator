# Study Guide: STAT 2011 — Exam 2 (Lecture 8: z-scores and the Normal Distribution)

> **Built from:** Lecture 8 notes (`lecture8-notes.md`), including the Exam 2 objectives listed in them
> **Assumptions:** This guide covers only Lecture 8. If Exam 2 also covers other lectures, you'll need to study those separately.

---

## 1. Overview

**What this exam covers:** The four Exam 2 objectives from Lecture 8: z-scores, the empirical rule (68-95-99.7), reading the standard normal table, and population vs. sample standard deviation.

**Study these first (highest priority):**
1. **Population vs. sample standard deviation (n − 1).** Your professor said forgetting n − 1 was the most common mistake on last year's exam.
2. **Computing and interpreting z-scores.** Everything else in this lecture builds on z.
3. **The empirical rule (68-95-99.7).** It's a quick way to answer "what percent of data falls between...?" questions.
4. **Reading the standard normal table.** Remember: the table gives the area to the **left** of z.

---

## 2. Key terms and definitions

| Term | Definition (from your materials) | In plain words |
|------|----------------------------------|----------------|
| z-score (z) | z = (x − μ) / σ; the number of standard deviations x is from the mean | How many "steps" of size σ a value is away from the average |
| Positive z | x is above the mean | The value is higher than average |
| Negative z | x is below the mean | The value is lower than average |
| μ (mu) | The mean, as used in the z formula and the population SD formula | The population average |
| σ (sigma) | Population standard deviation: σ = sqrt( Σ(x − μ)² / N ) | The typical distance from the average, for a whole population |
| s | Sample standard deviation: s = sqrt( Σ(x − x̄)² / (n − 1) ) | The typical distance from the average, for a sample. Divide by n − 1, not n |
| x̄ (x-bar) | The sample mean, used in the formula for s | The average of your sample |
| N / n | N = population size (in σ); n = sample size (in s) | How many values you have |
| Empirical rule | For a normal distribution, about 68% of data is within 1σ, 95% within 2σ, and 99.7% within 3σ of the mean | The 68-95-99.7 shortcut for bell-shaped data |
| Standard normal table | Gives the area to the LEFT of z, e.g. P(Z < 1.00) = 0.8413 | Look up z, and you get the proportion of values below it |

---

## 3. Main concepts

### 3.1 z-scores (Objective 1)
**What it is:** A z-score tells you how many standard deviations a value x is from the mean. You find it with z = (x − μ) / σ.

**Why it matters:** z-scores put different values on the same scale. You also need z to use the standard normal table.

**Example (from class):** Exam scores have μ = 72 and σ = 8. A score of 88 gives z = (88 − 72) / 8 = 16 / 8 = 2.0. So 88 is 2 standard deviations **above** the mean.

**Remember:** The sign tells you the direction. Positive means above the mean, and negative means below it.

### 3.2 The empirical rule, 68-95-99.7 (Objective 2)
**What it is:** For a normal (bell-shaped) distribution:
- about **68%** of the data is within **1σ** of the mean (between μ − σ and μ + σ)
- about **95%** is within **2σ**
- about **99.7%** is within **3σ**

**Why it matters:** You can estimate percentages fast, with no table needed.

**Example (example created for practice, using the class numbers μ = 72, σ = 8):**
- About 68% of scores are between 72 − 8 = **64** and 72 + 8 = **80**.
- About 95% are between 72 − 16 = **56** and 72 + 16 = **88**.
- About 99.7% are between 72 − 24 = **48** and 72 + 24 = **96**.

**One-tail trick (general background — not from your materials):** The normal curve is symmetric, so the part *outside* a range splits evenly between the two tails. For example, 95% are within 2σ, so 5% are outside, and about 2.5% are above μ + 2σ.

**Remember:** 1σ → 68%, 2σ → 95%, 3σ → 99.7%. This rule works only for normal (bell-shaped) data.

### 3.3 The standard normal table (Objective 3)
**What it is:** The table takes a z-score and gives you the **area to the left** of it. That area is the proportion (probability) of values below z. Your notes give one value: **P(Z < 1.00) = 0.8413**.

**Why it matters:** It gives exact probabilities, while the empirical rule gives only rough ones.

**How to use it:**
1. Turn x into z with z = (x − μ) / σ.
2. Look up z in the table. That gives P(Z < z), the area to the left.
3. If you need the area to the **right**, use 1 − (table value). *(general background — not from your materials: the total area under the curve is 1)*

**Example (example created for practice):** Exam scores have μ = 72 and σ = 8. What proportion of students scored below 80?
- z = (80 − 72) / 8 = 8 / 8 = 1.00
- P(Z < 1.00) = 0.8413, so about **84.13%** scored below 80.
- About 1 − 0.8413 = **0.1587** (15.87%) scored above 80.

**Remember:** The table gives the area to the LEFT. If you want the area to the right, subtract from 1.

### 3.4 Population vs. sample standard deviation (Objective 4)
**What it is:** There are two formulas for standard deviation:
- **Population (σ):** use it when you have **every** member of the group. Divide by **N**.
- **Sample (s):** use it when you have only **part** of the group. Divide by **n − 1**.

**Why it matters:** Your professor said: "Don't forget n − 1 for samples! Most common mistake on last year's exam."

**Example (example created for practice):** See the worked example in Section 4. For the same data, s ≈ 1.5811 and σ ≈ 1.4142.

**Remember:** Is it a sample? Then use s and divide by n − 1. Dividing by n − 1 makes s a little larger than σ for the same numbers.

---

## 4. Formulas

### Which formula do I use?

| The question asks... | Use |
|----------------------|-----|
| "How many standard deviations from the mean?" or "Compare scores on different scales" | z = (x − μ) / σ |
| "About what percent is between...?" (normal data, values exactly 1, 2, or 3 σ away) | Empirical rule (68-95-99.7) |
| "What proportion is below / above x?" (exact) | z-score, then the standard normal table |
| "Find the SD" and the data is a **sample** | s, divide by n − 1 |
| "Find the SD" and the data is the **whole population** | σ, divide by N |

### z-score
$$ z = \frac{x - \mu}{\sigma} $$

| Symbol | Meaning |
|--------|---------|
| z | z-score: the number of standard deviations x is from the mean |
| x | The value you're looking at |
| μ | The mean |
| σ | The standard deviation |

**Use it when:** A problem gives you a value, a mean, and a standard deviation, and asks how unusual the value is, how it compares to another one, or asks for a probability.

**Worked example (from class):**
1. Known values: x = 88, μ = 72, σ = 8.
2. Plug in: z = (88 − 72) / 8.
3. Calculate: 88 − 72 = 16, and 16 / 8 = 2.0.
4. Interpret: a score of 88 is 2.0 standard deviations above the mean.

### Sample standard deviation
$$ s = \sqrt{\frac{\sum (x - \bar{x})^2}{n - 1}} $$

| Symbol | Meaning |
|--------|---------|
| s | Sample standard deviation |
| x | Each data value |
| x̄ | The sample mean |
| Σ | "Add them all up" |
| n | The number of values in the sample |

**Use it when:** Your data is a sample, meaning part of a bigger group.

**Worked example (example created for practice):** The data are 4, 8, 6, 5, 7, and this is a sample.
1. Find the mean: x̄ = (4 + 8 + 6 + 5 + 7) / 5 = 30 / 5 = 6.
2. Subtract the mean from each value: −2, 2, 0, −1, 1.
3. Square each one: 4, 4, 0, 1, 1.
4. Add them up: Σ(x − x̄)² = 10.
5. Divide by n − 1 = 4: 10 / 4 = 2.5.
6. Take the square root: s = √2.5 ≈ **1.5811**.
7. Interpret: values in this sample are typically about 1.58 away from the mean of 6.

### Population standard deviation
$$ \sigma = \sqrt{\frac{\sum (x - \mu)^2}{N}} $$

| Symbol | Meaning |
|--------|---------|
| σ | Population standard deviation |
| x | Each data value |
| μ | The population mean |
| N | The number of values in the population |

**Use it when:** Your data is the whole population.

**Worked example (example created for practice):** Suppose 4, 8, 6, 5, 7 is the entire population.
1. Steps 1–4 are the same as above: μ = 6, and Σ(x − μ)² = 10.
2. Divide by N = 5: 10 / 5 = 2.
3. Take the square root: σ = √2 ≈ **1.4142**.
4. Interpret: σ (1.4142) is smaller than s (1.5811) because you divided by 5 instead of 4.

---

## 5. Common mistakes

| Mistake | Why it's wrong | Do this instead |
|---------|----------------|-----------------|
| Dividing by n instead of n − 1 for a sample | The sample formula uses n − 1. Your professor called this the most common mistake on last year's exam | Ask yourself "sample or population?" before you start. For a sample, use n − 1 |
| Computing (μ − x) / σ instead of (x − μ) / σ | This flips the sign, so above-mean values look like they're below | Always subtract the **mean from the value**: x − μ |
| Reading the table value as the area to the right | The table gives the area to the **left** of z | For "greater than," use 1 − (table value) |
| Forgetting the square root in s or σ | Without it, you get the variance, not the standard deviation | Do the square root as your last step |
| Using the empirical rule for any value | It works only at exactly 1, 2, or 3 σ, and only for normal data | For other z values, use the table |
| Rounding too early | Small rounding errors add up | Keep full decimals until the final answer |
| Saying "z = −1.5 means 1.5 points below" | z counts **standard deviations**, not points | Say "1.5 standard deviations below the mean" |

---

## 6. Practice questions

*Try these before you look at the answer key.*

**Multiple choice**

1. [Easy] A student's z-score is −1.5. What does this mean?
   a) The score is 1.5 points below the mean
   b) The score is 1.5 standard deviations below the mean
   c) The score is 1.5 standard deviations above the mean
   d) The score is 15% below the mean

2. [Easy] For a normal distribution, about what percent of data falls within 2 standard deviations of the mean?
   a) 68% b) 95% c) 99.7% d) 50%

3. [Easy] The standard normal table gives the area:
   a) to the right of z b) between −z and z c) to the left of z d) above the mean

4. [Medium] You measure the heights of 25 students to describe all 300 students in a class. Which standard deviation formula should you use?
   a) σ, dividing by N b) σ, dividing by n − 1 c) s, dividing by n d) s, dividing by n − 1

**Short answer / calculation**

5. [Easy] Exam scores have μ = 72 and σ = 8. Find the z-score for a score of 60 and explain what it means.

6. [Medium] Heights in a group are normal with μ = 65 inches and σ = 3 inches *(example created for practice)*. Between which two heights do about 95% of people fall?

7. [Medium] Exam scores are normal with μ = 72 and σ = 8. Using the empirical rule, about what percent of students scored between 64 and 80?

8. [Medium] Exam scores are normal with μ = 72 and σ = 8. Using the standard normal table (P(Z < 1.00) = 0.8413), what proportion of students scored **below** 80?

9. [Medium] Here is a sample: 2, 4, 4, 6, 9. Find the sample standard deviation s.

**Problem / scenario**

10. [Challenge] Use the same numbers as Question 9 (2, 4, 4, 6, 9), but now they are the **entire population**. Find σ. Which is larger, s or σ, and why?

11. [Challenge] Exam scores are normal with μ = 72 and σ = 8. What proportion of students scored **above** 80?

12. [Challenge] Ana scored 84 on Exam A (μ = 72, σ = 8). Ben scored 75 on Exam B (μ = 65, σ = 5) *(example created for practice)*. Relative to their own class, who did better? Show your z-scores.

---

## 7. Answer key with explanations

1. **Answer:** b
   **Why:** z counts standard deviations from the mean, and a negative sign means below the mean (Section 3.1).
   **Common trap:** (a) treats z as raw points. z is in standard deviations, not points.

2. **Answer:** b) 95%
   **Why:** Empirical rule: 68% within 1σ, 95% within 2σ, 99.7% within 3σ (Section 3.2).
   **Common trap:** 68% is for 1σ, and 99.7% is for 3σ.

3. **Answer:** c
   **Why:** Your notes say the table gives the area to the LEFT of z (Section 3.3).
   **Common trap:** (a). For a right-side area, you have to compute 1 − (table value) yourself.

4. **Answer:** d
   **Why:** 25 students are part of the class, so this is a sample. Use s and divide by n − 1 (Section 3.4).
   **Common trap:** (c), dividing by n. This is the mistake your professor warned about.

5. **Answer:** z = −1.5
   **Steps:** z = (60 − 72) / 8 = −12 / 8 = −1.5.
   **Meaning:** A score of 60 is 1.5 standard deviations **below** the mean.
   **Common trap:** Doing 72 − 60 and getting +1.5. Always compute x − μ.

6. **Answer:** About 59 to 71 inches
   **Steps:** 95% → within 2σ. 2σ = 2 × 3 = 6. Low end: 65 − 6 = 59. High end: 65 + 6 = 71.
   **Common trap:** Using 1σ (62 to 68). That range covers about 68%, not 95%.

7. **Answer:** About 68%
   **Steps:** 64 = 72 − 8 = μ − 1σ, and 80 = 72 + 8 = μ + 1σ. "Within 1σ" → about 68% (Section 3.2).
   **Common trap:** Choosing 95%. Check how many σ away the endpoints are first.

8. **Answer:** 0.8413 (about 84.13%)
   **Steps:** z = (80 − 72) / 8 = 8 / 8 = 1.00. The table gives the area to the left: P(Z < 1.00) = 0.8413.
   **Common trap:** Answering 0.1587. That's the area to the right, not the left.

9. **Answer:** s = √7 ≈ 2.6458
   **Steps:**
   1. x̄ = (2 + 4 + 4 + 6 + 9) / 5 = 25 / 5 = 5.
   2. Deviations: −3, −1, −1, 1, 4.
   3. Squared: 9, 1, 1, 1, 16. Sum = 28.
   4. Divide by n − 1 = 4: 28 / 4 = 7.
   5. s = √7 ≈ 2.6458.
   **Common trap:** Dividing by 5 (gives 2.3664) or forgetting the square root (gives 7).

10. **Answer:** σ = √5.6 ≈ 2.3664. s (2.6458) is larger.
    **Steps:** The sum of squared deviations is still 28 (from Question 9). Divide by N = 5: 28 / 5 = 5.6. σ = √5.6 ≈ 2.3664.
    **Why s is larger:** s divides by a smaller number (n − 1 = 4 instead of 5), so the result is bigger (Section 3.4).
    **Common trap:** Thinking the two formulas always give the same answer. They differ only in the denominator, but that changes the result.

11. **Answer:** 0.1587 (about 15.87%)
    **Steps:**
    1. z = (80 − 72) / 8 = 1.00.
    2. The table gives the area to the left: P(Z < 1.00) = 0.8413.
    3. Area to the right = 1 − 0.8413 = 0.1587 *(general background — not from your materials: the total area under the curve is 1)*.
    **Common trap:** Stopping at 0.8413. That answers "below 80," not "above 80."

12. **Answer:** Ben did better relative to his class.
    **Steps:** Ana: z = (84 − 72) / 8 = 12 / 8 = 1.5. Ben: z = (75 − 65) / 5 = 10 / 5 = 2.0.
    **Why:** Ben is 2.0 standard deviations above his mean, and Ana is only 1.5 above hers (Section 3.1).
    **Common trap:** Picking Ana because 84 > 75. Raw scores on different exams can't be compared directly, so compare z-scores.

---

## 8. Final review checklist

- [ ] I can define z-score, μ, σ, s, x̄, N, and n in my own words.
- [ ] I can compute a z-score and say what its sign and size mean.
- [ ] I can use the empirical rule to find the ranges for 68%, 95%, and 99.7% of the data.
- [ ] I can turn a value into z and use the standard normal table to find the area to the left, and use 1 − (table value) for the area to the right.
- [ ] I can tell whether data is a sample or a population and pick s (n − 1) or σ (N).
- [ ] I can compute s and σ step by step without forgetting the square root.
- [ ] I can avoid the mistakes listed in Section 5.
- [ ] I got at least 80% of the practice questions right without looking.

---

## 9. Gaps to check

- **Only one table value is given.** Your notes list P(Z < 1.00) = 0.8413 but don't include the full standard normal table. Get the table your class uses and practice reading other z values.
- **Right-tail and "between" areas aren't covered.** The notes say only that the table gives the area to the left. This guide uses 1 − (table value) for right-tail areas (general background). Check whether your professor wants you to find areas between two z values, or to use symmetry for negative z.
- **z-scores with a sample.** The notes give z only with μ and σ. Ask whether the exam will also use x̄ and s in the z formula.
- **Rounding rules.** The notes don't say how many decimal places to use for z or probabilities (the table uses two for z and four for areas).
- **Exam 2 scope.** These notes cover Lecture 8 only. Check whether Exam 2 includes other lectures.
