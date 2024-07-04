# Keeping Users Engaged During Repeated Interviews by a Virtual Agent: Using Large Language Models to Reliably Diversify Questions

This GitHub repository provides the supplementary materials.
As part of the supplementary materials, we include the LLM-generated item (question) variants and content we included in the ITEM VARIANTS PLUS condition. Also, we provide the implementation details and the prompts used to generate the item (question) variants and conversational contents. Lastly, we provide details of the response values, satisfaction ratings, and perception ratings participants provided when interacting with the agent over the course of 14 days.

## Prompts

You can find the prompts in the [`PROMPTS.md`](PROMPTS.md) file.

## LLM-Generated Content

All contents used in the validation study can be found in the `llm_outputs` folder as csv files.
Please refer to the [`OUTPUTS.md`](llm_outputs/OUTPUTS.md) file for the descriptions and generation details of the contents.

## Participant Responses

During the two-week validation study, participants answered questions administered by the agent. 

The [`responses_table.pdf`](responses_table.pdf) provides the percentage of response values for each PROMIS Depression questions across all three conditions. The table also factors in days that the participants did not interact with the agent or skipped to answer.

## Participant Perceptions

During the two-week validation study, participants answered questions about their satisfaction and perception of the agent.

The [`longitudinal.pdf`](longitudinal.pdf) shows the changes in satisfaction and perception (`desire to continue talking with the agent`, `naturalness`, and `repetitiveness`) of the agent throughout the 14-day study interaction period for each of the three study conditions. 

> Line graphs showing the mean agent satisfaction, desire to continue talking to the agent, naturalness of the agent, and repetitiveness of the agent from 1 to 7 on the Y axis against the number of visits or days in the study from 1 to 14 on the X axis. Three line graphs are shown for each study condition consisting of four lines each. The CONTROL condition overall had the highest repetitiveness numbers ranging from 4.5 to 6 across the two weeks. All other conditions and lines were fairly consistent ranging from 3 to 5.

## Citation

```bibtex
@inproceedings{yun2024keeping,
author = {Yun, Hye Sun and Arjmand, Mehdi and Sherlock, Phillip and Paasche-Orlow, Michael and Griffith, James W. and Bickmore, Timothy},
title = {Keeping Users Engaged During Repeated Interviews by a Virtual Agent: Using Large Language Models to Reliably Diversify Questions},
year = {2024},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/10.1145/3652988.3673929},
doi = {10.1145/3652988.3673929},
booktitle = {Proceedings of the 24th ACM International Conference on Intelligent Virtual Agents},
location = {, Glasgow, United Kingdom, },
series = {IVA '24}
}
```