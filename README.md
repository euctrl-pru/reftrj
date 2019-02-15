# Reference trajectories for Performance Review of European ANS

This repository serves as a starting point to access the Reference Trajectory dataset.

The Reference Trajectory is a dataset produced by the PRU in order to make it possible for its stakeholders to
compute Performance Indicators (and as such replicate or complement the ones published by the PRU.)

# Data download

You can download the linked files using Google's `gsutil` for example in `data-raw` directory as:

```shell
```{bash, eval=FALSE}
$ gsutil https://storage.googleapis.com/pru-trajectories/sources/merged/overnight_cpr_fr24/raw_cpr_fr24_positions_2017-08-08.csv.bz2 data-raw/
```
```

# Reference Trajectory Data Set

## Flights

| Description                                             | type      | Year | Month | Day | URL              | Size (approx) |
|---------------------------------------------------------|-----------|------|-------|-----|------------------|---------------|
| Reference Trajectory flights on Aug 1, 2017             | flight    | 2017 |    08 |  01 | [URL][f20180801] | 400 KB        |
| Reference Trajectory flights on Aug 2, 2017             | flight    | 2017 |    08 |  02 | [URL][f20180802] | 400 KB        |
| Reference Trajectory flights on Aug 3, 2017             | flight    | 2017 |    08 |  03 | [URL][f20180803] | 400 KB        |

[f20180801]: https://storage.googleapis.com/pru-trajectories/sources/merged/overnight_cpr_fr24/cpr_fr24_events_2017-08-01.csv.bz2 "reference trajectory flights on 20180801"
[f20180802]: https://storage.googleapis.com/pru-trajectories/sources/merged/overnight_cpr_fr24/cpr_fr24_events_2017-08-02.csv.bz2 "reference trajectory flights on 20180802"
[f20180803]: https://storage.googleapis.com/pru-trajectories/sources/merged/overnight_cpr_fr24/cpr_fr24_events_2017-08-03.csv.bz2 "reference trajectory flights on 20180803"

## Positions

| Description                                             | type      | Year | Month | Day | URL              | Size (approx) |
|---------------------------------------------------------|-----------|------|-------|-----|------------------|---------------|
| Reference Trajectory synthetic positions on Aug 1, 2017 | positions | 2017 |    08 |  01 | [URL][p20180801] | 2.9 GB        |
| Reference Trajectory synthetic positions on Aug 2, 2017 | positions | 2017 |    08 |  02 | [URL][p20180802] | 2.9 GB        |
| Reference Trajectory synthetic positions on Aug 3, 2017 | positions | 2017 |    08 |  03 | [URL][p20180803] | 2.9 GB        |

[p20180801]: https://storage.googleapis.com/pru-trajectories/products/synth_positions/cpr_fr24/mas_05_cpr_fr24_synth_positions_2017-08-01.csv.bz2 "reference trajectory positions on 20180801"
[p20180802]: https://storage.googleapis.com/pru-trajectories/products/synth_positions/cpr_fr24/mas_05_cpr_fr24_synth_positions_2017-08-02.csv.bz2 "reference trajectory positions on 20180802"
[p20180803]: https://storage.googleapis.com/pru-trajectories/products/synth_positions/cpr_fr24/mas_05_cpr_fr24_synth_positions_2017-08-03.csv.bz2 "reference trajectory positions on 20180803"

# Documentation

| Description                                             | type      | URL              | Size (approx) |
|---------------------------------------------------------|-----------|------------------|---------------|
| Final report on RT project                              | PDF       | [URL][rtdoc1]    | 1.7 MB        |
| Optomized pipeline                                      |           | URL              |               |

[rtdoc1]: https://github.com/euctrl-pru/reftrj/raw/master/Trajectories_Production_Final_Report.pdf "Final report on RT project"



# Software

The software for the production of the Reference Trajectory dataset is written in Python (with some optimization pieces in C++).
We make this software available in the interest of feedback and exchanges with the aviation community at large.
We are very much interested in proposals for improvements.


