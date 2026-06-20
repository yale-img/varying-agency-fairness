# Effects of Time-Varying Perceived Agency on Fairness
Code and data for the paper "Effects of Time-Varying Perceived Agency on Fairness Judgments Towards Robots." If you use this data or code, please cite:

```latex
@inproceedings{shin26-varying-agency-fairness,
  author    = {Inyoung Shin and Houston Claure and Mai Blaustein and J. Gregory Trafton and Marynel V\'azquez},
  title     = {Effects of Time-Varying Perceived Agency on Fairness Judgments Towards Robots},
  booktitle = {Proceedings of the 35th IEEE International Conference on Robot and Human Interactive Communication (RO-MAN)},
  year      = {2026},
}
```

## Experimental Conditions

Participants were randomly assigned to one of four conditions:

| Scenario ID | Condition |
|------------|------------|
| 1A | High Agency → High Agency |
| 1B | High Agency → Low Agency |
| 2A | Low Agency → High Agency |
| 2B | Low Agency → Low Agency |

For a description of the prompts used in each scenario, please see [`survey/Phases.md`](survey/Phases.md). For a visual look of the survey, see [`survey/survey-example-highPA-lowPA.png`](survey/survey-example-highPA-lowPA.png).

The sections below describe the columns in the dataset [`dataset/experimentdata.csv`](dataset/experimentdata.csv). For the analysis code, see [`data_analysis_code/codes_data_anlaysis.ipynb`](data_analysis_code/codes_data_anlaysis.ipynb).

### Administrative Variables

| Variable | Description |
|-----------|-------------|
| duration | Survey duration (seconds) |
| scenarioID | Experimental condition (1A = High–High, 1B = High–Low, 2A = Low–High, 2B = Low–Low) |

### Attention Checks

| Variable | Description |
|-----------|-------------|
| phase1_Attencheck | Phase 1 Scenario attention check (1=True, 2=False) |
| Q74_2 | Phase 1 instructional attention check |
| Q13 | Phase 2 Scenario  (1=True, 2=False) |
| Q76_4 | Phase 2 instructional attention check |

### Fairness Measures

#### Phase 1

| Variable | Description |
|-----------|-------------|
| Q8 | Fairness rating (1–5 scale, 1= very unfair; 5=very fair)|
| Q81 | Open-ended fairness explanation |

#### Phase 2

| Variable | Description |
|-----------|-------------|
| Q16 | Fairness rating (1–5 scale) |
| Q83 | Open-ended fairness explanation |

### Blame Attribution

| Variable | Description |
|-----------|-------------|
| Q82_1 | Phase 1 blame attribution (0–10 scale) |
| Q84_1 | Phase 2 blame attribution (0–10 scale) |

### Trust Measures

All trust items use a 1–8 scale. A value of 9 indicates "Not Applicable."

#### Phase 1

| Variable | Description |
|-----------|-------------|
| Q73_1 | Performance Trust Item 1 |
| Q73_2 | Performance Trust Item 2 |
| Q73_6 | Performance Trust Item 3 |
| Q73_7 | Performance Trust Item 4 |
| Q73_3 | Moral Trust Item 1 |
| Q73_4 | Moral Trust Item 2 |
| Q73_5 | Moral Trust Item 3 |
| Q73_8 | Moral Trust Item 4 |
| Q73_9 | Moral Trust Item 5 |
| Q73_10 | Moral Trust Item 6 |

#### Phase 2

| Variable | Description |
|-----------|-------------|
| Q75_1 | Performance Trust Item 1 |
| Q75_2 | Performance Trust Item 2 |
| Q75_6 | Performance Trust Item 3 |
| Q75_7 | Performance Trust Item 4 |
| Q75_3 | Moral Trust Item 1 |
| Q75_4 | Moral Trust Item 2 |
| Q75_5 | Moral Trust Item 3 |
| Q75_8 | Moral Trust Item 4 |
| Q75_9 | Moral Trust Item 5 |
| Q75_10 | Moral Trust Item 6 |

### Perceived Agency (PA)

#### Phase 1

| Variable | Description |
|-----------|-------------|
| Q74_1 | PA Item 1 (1–5 scale) |
| Q74_3 | PA Item 2 (1–5 scale) |
| Q74_4 | PA Item 3 (1–5 scale) |
| Q74_5 | PA Item 4 (1–5 scale) |

#### Phase 2

| Variable | Description |
|-----------|-------------|
| Q76_1 | PA Item 1 (1–5 scale) |
| Q76_2 | PA Item 2 (1–5 scale) |
| Q76_3 | PA Item 3 (1–5 scale) |
| Q76_5 | PA Item 4 (1–5 scale) |

### Timing Variables

| Variable | Description |
|-----------|-------------|
| Q68_First Click | First click time |
| Q68_Last Click | Last click time |
| Q68_Page Submit | Page submission time |
| Q68_Click Count | Number of clicks recorded |

### Demographics

| Variable | Description |
|-----------|-------------|
| Q78 | Age |
| Q79 | Gender |
| Q79_5_TEXT | Self-described gender |
| Education | Educational attainment |

#### Education Coding

| Code | Category |
|------|----------|
| 1 | Less than primary school |
| 2 | Primary school |
| 3 | Some secondary school |
| 4 | Secondary school |
| 5 | Vocational or similar training |
| 6 | Some university, no degree |
| 7 | Bachelor's degree |
| 8 | Master's degree |
| 9 | Graduate or professional degree |
| 10 | Prefer not to say |

## Data Notes
- Participants completed two phases of the experiment.
- Fairness, blame, trust, and PA were measured after each phase.
- Open-ended responses were collected to supplement quantitative measures.
- Attention checks were included to ensure data quality.

## License

- **Code** in [`data_analysis_code/`](data_analysis_code/) is licensed under the [MIT License](data_analysis_code/LICENSE).
- **Data** in [`dataset/`](dataset/) is licensed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](dataset/LICENSE-DATA).

If you use this code or data, please cite the paper at the top of this readme.
