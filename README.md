# Szeged Weather Prediction with Deep Learning

Final project for the **Deep Learning (Discussion Seminar)** course.

## Course Information

- **Course:** Deep Learning (Discussion Seminar)
- **Subject code:** DL_BDS
- **Study program:** Master, 2nd Year, Big Data Science
- **Class group:** ds/DL/MiBDS - 2nd Year
- **Lecturer:** Pamela Krzypkowska BA
- **Language of instruction:** English
- **Assessment form:** Pass with a grade
- **ECTS:** 4

## Team

- Youngjun Son
- Emma Hope

## Project Overview

The goal of this project is to predict the next-day temperature using the previous 72 hours of hourly weather data.

Although the original project option was based on the Szeged weather prediction task, the final implementation uses hourly weather data collected through Open-Meteo for Szeged and five nearby cities:

- Szeged
- Budapest
- Debrecen
- Pecs
- Belgrade
- Timisoara

The project treats weather prediction as a regression problem and compares a persistence baseline with recurrent neural network models.

## Models

- Persistence baseline
- Vanilla LSTM
- GRU

The GRU model achieved the best overall performance in our experiments, with strong predictive accuracy and low bias.

## Key Methods

- Chronological train/validation/test split
- Feature normalization
- Wind direction transformation using sine and cosine components
- 72-hour sliding input window
- Next-24-hour average temperature target
- Manual early stopping in PyTorch
- Stability check across multiple random seeds

## Repository Contents

```text
Deep_Learning_Project.ipynb       Final Jupyter notebook
presentation_slide.pdf            Final presentation slides
data/meteostat/*.csv              Hourly weather datasets used in the notebook
checkpoints/*.pt                  Saved best model checkpoints
README.txt                        Submission note
```

## AI Tools Disclosure

Generative AI tools were used as support for debugging, checking explanations, improving presentation wording, and preparing final submission materials. The project team reviewed and understood the code, metrics, and conclusions.
