# Reference Trajectories for Performance Review of European ANS

This repository serves as a starting point to access the Reference Trajectory dataset.

The Reference Trajectory is a dataset produced by the PRU in order to make it possible for its stakeholders to
compute Performance Indicators (and as such replicate or complement the ones published by the PRU.)

# Data download

You can download the linked files either by clicking and saving them or
by using Google's `gsutil` as (it saves in  `data-raw` directory):

```shell
$ gsutil https://storage.googleapis.com/pru-trajectories/sources/merged/overnight_cpr_fr24/raw_cpr_fr24_positions_2017-08-08.csv.bz2 data-raw/
```

# Reference Trajectory Data Set

## Flights

| Description           | type      | Year | Month | Day | URL              | Size (approx) |
|-----------------------|-----------|------|-------|-----|------------------|---------------|
| RT flights            | flight    | 2017 |    08 |  01 | [URL][f20180801] | 400 KB        |
| RT flights            | flight    | 2017 |    08 |  02 | [URL][f20180802] | 400 KB        |
| RT flights            | flight    | 2017 |    08 |  03 | [URL][f20180803] | 400 KB        |

[f20180801]: https://storage.googleapis.com/pru-trajectories/sources/merged/overnight_cpr_fr24/cpr_fr24_events_2017-08-01.csv.bz2 "reference trajectory flights on 20180801"
[f20180802]: https://storage.googleapis.com/pru-trajectories/sources/merged/overnight_cpr_fr24/cpr_fr24_events_2017-08-02.csv.bz2 "reference trajectory flights on 20180802"
[f20180803]: https://storage.googleapis.com/pru-trajectories/sources/merged/overnight_cpr_fr24/cpr_fr24_events_2017-08-03.csv.bz2 "reference trajectory flights on 20180803"

## Positions

| Description   | type      | Year | Month | Day | URL              | Size    |
|---------------|-----------|------|-------|-----|------------------|---------|
| RT positions  | positions | 2017 |    08 |  01 | [URL][p20180801] | 2.9 GB  |
| RT positions  | positions | 2017 |    08 |  02 | [URL][p20180802] | 2.9 GB  |
| RT positions  | positions | 2017 |    08 |  03 | [URL][p20180803] | 2.9 GB  |

[p20180801]: https://storage.googleapis.com/pru-trajectories/products/synth_positions/cpr_fr24/mas_05_cpr_fr24_synth_positions_2017-08-01.csv.bz2 "reference trajectory positions on 20180801"
[p20180802]: https://storage.googleapis.com/pru-trajectories/products/synth_positions/cpr_fr24/mas_05_cpr_fr24_synth_positions_2017-08-02.csv.bz2 "reference trajectory positions on 20180802"
[p20180803]: https://storage.googleapis.com/pru-trajectories/products/synth_positions/cpr_fr24/mas_05_cpr_fr24_synth_positions_2017-08-03.csv.bz2 "reference trajectory positions on 20180803"

# Documentation

| Description                                             | type      | URL              | Size (approx) |
|---------------------------------------------------------|-----------|------------------|---------------|
| Final report on RT project                              | PDF       | [URL][rtdoc1]    | 1.7 MB        |
| Optimized pipeline                                      | PDF       | [URL][rtdoc2]    | 0.6 MB        |

[rtdoc1]: https://github.com/euctrl-pru/reftrj/raw/master/Trajectories_Production_Final_Report.pdf "Final report on RT project"
[rtdoc2]: <https://github.com/euctrl-pru/reftrj/blob/master/Trajectories%20Pipeline%20User%20Guide%20issue%201_0_0.pdf> "Optimized pipeline"



# Software

The software for the production of the Reference Trajectory dataset is written in Python (with some optimization pieces in C++).
We make this software available in the interest of feedback and exchanges with the aviation community at large.
We are very much interested in proposals for improvements.

* `rt-python`: Python code for the production of Reference Trajectories, [repo URL][rt-python].
  Developed by Via Technology for the PRU of [EUROCONTROL<img src='https://upload.wikimedia.org/wikipedia/commons/b/b2/Eurocontrol_logo_2010.svg' height='20px'>][euctrl] and made openly available. 
* `via-sphere`: An header-only C++ library with Python bindings for calculating distances, angles and positions on
  the surface of a sphere, [repo URL][via-sphere].
  Developed and made openly available by [Via Technology<img src='https://via-technology.aero/wp-content/uploads/2017/07/Via-Technology-x2.png' height='14px'>][via].

[rt-python]: <https://github.com/euctrl-pru/rt-python> "rt-python repository"
[via-sphere]: <https://bitbucket.org/viaaero/via-sphere/src/master/>
[via]: <https://via-technology.aero/> "Via Technology's Home Page"
[euctrl]: <https://www.eurocontrol.int/> "EUROCONTROL's Home Page"

# License

The data and the documentation are licensed under **CC0-1.0**.

The software is licensed under MIT or as stated in the relevant repository.

# Citation
Please cite this work as

```
@inproceedings{,
  author = {Spinielli, Enrico and Koelle, Rainer and Barker, Ken and Korbey, Nicholas},
  title = {Open {{Flight Trajectories}} for {{Reproducible ANS Performance Review}}},
  location = {{Salzburg, Austria}},
  url = {https://www.sesarju.eu/sites/default/files/documents/sid/2018/papers/SIDs_2018_paper_4.pdf},
  eventtitle = {{{SESAR Innovation Days}} 2018},
  date = {2018},
  pages = {8}
}
```

