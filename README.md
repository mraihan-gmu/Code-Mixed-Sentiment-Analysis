# Code-Mixed-Sentiment-Analysis
This is a dataset for the sentiment analysis task. It contains 100k code mixed data. The languages are Bangla-English-Hindi.

### Dataset Generation:

Initially, we select the Amazon Review Dataset as our base data, referenced from Ni et al. (2019)[^1]. We randomly extract 100,000 instances from this dataset. The original labels in this dataset are ratings, scaled from 1 to 5. For our specific task, we categorize them into Positive (rating > 3), Neutral (rating = 3), and Negative (rating < 3), ensuring a balanced number of instances for each label. To generate the synthetic Code-mixed dataset, we apply two distinct methodologies: the Random Code-mixing Algorithm by Krishnan et al. (2021)[^2] and r-CM by Santy et al. (2021)[^3].

### Class Distribution:

#### For train.csv:

| Label    | Count | Percentage |
|----------|-------|------------|
| Negative | 20000 | 33.33%     |
| Neutral  | 20000 | 33.33%     |
| Positive | 19999 | 33.33%     |

#### For dev.csv:

| Label    | Count | Percentage |
|----------|-------|------------|
| Neutral  | 6667  | 33.34%     |
| Positive | 6667  | 33.34%     |
| Negative | 6666  | 33.33%     |

#### For test.csv:

| Label    | Count | Percentage |
|----------|-------|------------|
| Negative | 6667  | 33.34%     |
| Positive | 6667  | 33.34%     |
| Neutral  | 6666  | 33.33%     |

### Cite our Paper:

If you utilize this dataset, kindly cite our paper.

```bibtex
@article{raihan2023mixed,
  title={Mixed-Distil-BERT: Code-mixed Language Modeling for Bangla, English, and Hindi},
  author={Raihan, Md Nishat and Goswami, Dhiman and Mahmud, Antara},
  journal={arXiv preprint arXiv:2309.10272},
  year={2023}
}
