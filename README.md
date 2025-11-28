- For searching xjtlu ics notes , goes to [XJTLU_ICS](https://github.com/Xyu-Chern/XJTLU_ICS)
- For cs336 my [implementation](https://github.com/Xyu-Chern/STF_CS336), the [vido](https://www.bilibili.com/video/BV14X41zZEPh/?spm_id_from=333.40164.top_right_bar_window_custom_collection.content.click&vd_source=2aae7a128408cb00e90d1288194e69d3) , the [link](https://stanford-cs336.github.io/spring2025/)
-
| | FQL | IFQL | DIFQL | MFQL | MFQL-BPTT | DMFQL |
|:---|:---:|:---:|:---:|:---:|:---:|:---:|
| **Forward Policy Call** | 13 | 1 | 1 | 11 | 21 | 11 |
| **Forward Value Call** | 3 | 4 | 5 | 3 | 4 | 4 |
| **Backward Policy Call** | 2 | 1 | 1 | 1 | 10 | 1 |
| **Backward Value Call** | 2 | 2 | 3 | 1 | 2 | 2 |
| **Total Calls** | 20 | 8 | 10 | 16 | 37 | 18 |
| **Actual Time in Minutes** | 37 | 29 | 31 | 35 | 61 | 37 |


| Metric | DMFQL(α=1) | DMFQL(α*) |
|--------|------------|-----------|
| antmaze-large-navigate-singletask-v0         | 72 ± 8 | 72 ± 8 |
| humanoidmaze-medium-navigate-singletask-v0      | 41 ± 17 | 44 ± 13 |
| humanoidmaze-large-navigate-singletask-v0      | 7 ± 3 | 7 ± 3 |
| antsoccer-arena-navigate-singletask-v0      | 38 ± 5 | 37 ± 5 |
| cube-single-play-singletask-v0      | 98 ± 1 | 98 ± 1 |
| cube-double-play-singletask-v0      | 72 ± 6 | 75 ± 6 |
| scene-play-singletask-v0     | 90 ± 8 | 91 ± 10 |
| puzzle-3x3-play-singletask-v0     | 6 ± 2 | 6 ± 2 |
| puzzle-4x4-play-singletask-v0      | 11 ± 6 | 14 ± 4 |
| Total     | 435 | 443 |

| | FQL* | MFQL | DMFQL | MFQL_bptt | MFFeBRAC | DMFReBRAC |
|:---|:---:|:---:|:---:|:---:|:---:|:---:|
| antmaze-large-navigate-singletask-v0   | $80 \pm 8$ | $62 \pm 11$ | $72 \pm 8$ | $64 \pm 13$ | $65 \pm 13$ | $83 \pm 7$ |
|humanoidmaze-medium-navigate-singletask-v0    | $19 \pm 12$ | $49 \pm 9$ | $44 \pm 13$ | $54 \pm 9$ | $53 \pm 14$ | $52 \pm 7$ |
|  humanoidmaze-large-navigate-singletask-v0 | $7 \pm 6$ | $8 \pm 3$ | $7 \pm 3$ | $6 \pm 2$ | $9 \pm 4$ | $8 \pm 2$ |
| antsoccer-arena-navigate-singletask-v0   | $39 \pm 6$ | $43 \pm 6$ | $37 \pm 5$ | $45 \pm 5$ | $91 \pm 5$ | $41 \pm 6$ |
|cube-single-play-singletask-v0 | $97 \pm 2$ | $95 \pm 1$ | $98 \pm 1$ | $62 \pm 37$ | $91 \pm 5$ | $99 \pm 1$ |
|cube-double-play-singletask-v0 | $36 \pm 6$ | $72 \pm 4$ | $75 \pm 6$ | $72 \pm 3$ | $74 \pm 4$ | $75 \pm 3$ |
| scene-play-singletask-v0| $76 \pm 9$ | $57 \pm 20$ | $90 \pm 10$ | $68 \pm 15$ | $57 \pm 12$ | $92 \pm 6$ |
| puzzle-3x3-play-singletask-v0 | $16 \pm 5$ | $7 \pm 3$ | $6 \pm 2$ | $1 \pm 1$ | $7 \pm 2$ | $5 \pm 2$ |
| puzzle-4x4-play-singletask-v0   | $11 \pm 3$ | $24 \pm 3$ | $14 \pm 4$ | $0 \pm 0$ | $25 \pm 5$ | $12 \pm 3$ |
| **Total** | **381** | **418** | **443** | **372** | **425** | **466** |
|pen-human-v1 | $53 \pm 6$ | $75 \pm 9$ | $72 \pm 8$ | - | $64 \pm 9$ | $74 \pm 8$ |
| pen-cloned-v1| $74 \pm 11$ | $75 \pm 9$ | $80 \pm 5$ | - | $71 \pm 12$ | $75 \pm 10$ |
| pen-expert-v1| $142 \pm 6$ | $138 \pm 4$ | $130 \pm 8$ | - | $140 \pm 9$ | $143 \pm 4$ |
| door-expert-v1| $104 \pm 1$ | $104 \pm 2$ | $104 \pm 1$ | - | $105 \pm 8$ | $105 \pm 1$ |
|hammer-expert-v1 | $125 \pm 3$ | $126 \pm 3$ | $124 \pm 5$ | - | $126 \pm 3$ | $126 \pm 1$ |
|relocate-expert-v1 | $107 \pm 1$ | $106 \pm 4$ | $104 \pm 4$ | - | $106 \pm 1$ | $107 \pm 2$ |
| **Total** | **605** | **623** | **614** | - | **614** | **630** |
