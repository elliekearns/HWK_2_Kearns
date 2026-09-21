# Dog Guessing Machine

## Purpose

Dog Guessing Machine is a small, playful classifier that predicts a likely dog breed from two inputs:

- size, from tiny to giant
- hair type: short, long, or curly

It is a learning activity, not a real dog-identification tool. The goal is to show how a model can compare an input with a small set of examples, make a prediction, and explain its decision.

## How to open and use the page

1. Find `dog-classifier.html` in this folder.
2. Double-click the file to open it in Chrome, Safari, Firefox, or another web browser.
3. Move the size slider and choose a hair-type icon.
4. Read the breed prediction and the explanation below it.
5. Try unusual combinations, such as tiny + long hair, to challenge the model.

No installation, account, API key, or build step is needed.

## How it makes a prediction

The classifier stores eight labeled examples, including Chihuahua, Bichon Frisé, Poodle, Golden Retriever, and Great Dane. Each example has a size and hair type.

For each visitor choice, the page calculates a **distance** to every stored example:

- A closer size gives a smaller distance.
- Matching hair type adds no extra distance.
- Different hair type adds 45 distance points.

The example with the smallest distance becomes the prediction. The page also shows the closest stored example and the distance score. Smaller scores mean a closer match.

When the distance is 20 or more, the page says the result is “not a great guess.” The model still chooses the least-bad label, but it admits that none of its examples fit well.

## A limitation I discovered

With only size and hair type, many very different dogs can look similar to the model. For example, a tiny dog with long hair may be closest to Lhasa Apso even when that does not make much sense. Instead of adding a label for every possible dog, this project uses a distance cutoff to show when the model is uncertain.

The model also does not see a real dog, understand breed biology, or use details such as color, ears, weight, or temperament.

## Short development log

- Started with a size slider and three hair-type choices.
- Added eight breed labels, including Bichon Frisé for tiny + curly and Golden Retriever for big + long.
- Added a visible distance score and an explanation of why the closest example won.
- Added a 20-point cutoff so weak matches are labeled “not a great guess.”
- Improved the page text to teach pattern matching, decision boundaries, and model limitations.
