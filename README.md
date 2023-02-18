# Train-Forcasting

## Reference
---

*   [Train Data](https://challengedata.ens.fr/participants/challenges/89/)


### Grouping Data
---

Grouping stations by there density to reduce number of variable names
Ex: High density, Medium density, low density

Getting average density for each station at a particular time
Get general statistics per station
Starting out, just P1Q0

Baseline Model

### Handling Null Values
---

*   **P&Q**

1)  235 rows that have 0 P&Q data
2)  Needs to be double checked
3)  Remove them if they have all nan

*   **P**

1)  Check if all 6am trains have no previous train data
2)  Potentially make all nan -> median (backed by graph notebook)

*   **q**

1)  Check if all 6am trains have no previous station data
2)  Potentially make all nan -> median (backed by graph notebook)

*   **Hour**

1)  based on train number
2)  pick the hour that has the majority of train numbers
3)  Fill in hour that has most votes for train number