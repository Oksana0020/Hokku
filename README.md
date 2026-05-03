# Hokku Generator (Genetic Algorithm)

## Overview

This project explores generating short Japanese-style three-line poems called **hokku** using a **Genetic Algorithm (GA)**.

A hokku is a short three-line poem that follows the traditional:

- 5 syllables  
- 7 syllables  
- 5 syllables  

pattern.

The algorithm searches for combinations of words that satisfy structural, grammatical, and stylistic rules.

---

## Main Features

- Generates three-line hokku poems
- Uses vocabulary divided into categories:
  - nouns
  - verbs
  - adjectives
  - adverbs
  - markers
  - season words
- Uses weighted cost function
- Uses tournament parent selection
- Uses category-based mutation
- Improves poems over generations

---

## Cost Function Rules

The GA evaluates each poem using penalties such as:

- wrong syllable counts
- missing marker
- bad marker position
- poor ending word
- repeated words
- weak grammar structure
- part of speech balance
- missing season word

**Lower cost = better poem**

---

## Genetic Algorithm Process

1. Create random population of poems  
2. Evaluate cost of each poem  
3. Select best parents  
4. Apply crossover  
5. Apply mutation  
6. Keep best solutions  
7. Repeat for many generations  

---

## Parameters

Example settings:

```python
population_size = 1000
generations = 300
child_rate = 0.6
mutation_rate = 0.15

---

## Example output

```python
old moon softly
misty river drifts —
spring wind lantern

---

## Results

Early versions reached cost = 0 easily
Final versions used more realistic rules
Final poems were close to valid hokku
GA performed well on creative constrained generation
AI can write poems but not as soul-touching as humans are!


---

##Future Improvements may include:

Larger vocabulary.
Variety of grammar rules.
Try roulette-wheel selection as an alternative to tournament selection. Compare selection methods.
Implement adaptive penalty weights that change over generations.
Compare generated poems against real hokku poems using similarity or language models.

---

Project was created as part of Artificial Intelligence (AI) coursework.
