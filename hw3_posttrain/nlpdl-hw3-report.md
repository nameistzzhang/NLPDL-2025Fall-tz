# NLPDL HW3 Report

### Zeroshot Qwen2.5-0.5B Best-of-N on GSM-8K

> overall setting:
> 
> 
> **temperature: 1.0
> top_p: 1.0**
> 

| experiment | format reward | answer reward | reward | correct_n | format_only_n | neither_n | total_n | time cost |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Best-of-1 | 0.2805 | 0.0015 | 0.0015 | 2 | 368 | 949 | 1319 | 00:36 |
| Best-of-2 | 0.2934 | 0.0106 | 0.0106 | 14 | 731 | 1893 | 2638 | 01:15 |
| Best-of-4 | 0.2813 | 0.0114 | 0.0114 | 15 | 1424 | 3837 | 5276 | 02:31 |
| Best-of-8 | 0.2881 | 0.0273 | 0.0273 | 38 | 2820 | 7694 | 10552 | 05:02 |
| Best-of-16 | 0.3139 |  0.0637 |  0.0637 | 91 | 5663 | 15350 | 21104 | 10:17 |
- HINT: you have to run the script by moving the zero-shot.py from ./src to the working directory and run it
- There seems to have some bug at model names (Qwen2.5-0.5B) and vLLM logprobs analyze