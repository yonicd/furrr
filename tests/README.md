Tests and Coverage
================
31 March, 2020 21:18:16

  - [Coverage](#coverage)
  - [Unit Tests](#unit-tests)

This output is created by
[covrpage](https://github.com/metrumresearchgroup/covrpage).

## Coverage

Coverage summary is created using the
[covr](https://github.com/r-lib/covr) package.

| Object                                                    | Coverage (%) |
| :-------------------------------------------------------- | :----------: |
| furrr                                                     |    55.50     |
| [R/future\_imap.R](../R/future_imap.R)                    |     0.00     |
| [R/future\_invoke\_map.R](../R/future_invoke_map.R)       |     0.00     |
| [R/future\_modify.R](../R/future_modify.R)                |     0.00     |
| [R/future\_walk.R](../R/future_walk.R)                    |     0.00     |
| [R/future\_pmap.R](../R/future_pmap.R)                    |    30.43     |
| [R/random-seeds.R](../R/random-seeds.R)                   |    30.77     |
| [R/utils.R](../R/utils.R)                                 |    36.04     |
| [R/future\_map2.R](../R/future_map2.R)                    |    38.46     |
| [R/fold.R](../R/fold.R)                                   |    43.33     |
| [R/future\_pmap\_template.R](../R/future_pmap_template.R) |    55.86     |
| [R/resolve.R](../R/resolve.R)                             |    58.33     |
| [R/load-balancer.R](../R/load-balancer.R)                 |    58.82     |
| [R/future\_map2\_template.R](../R/future_map2_template.R) |    58.88     |
| [R/future\_map.R](../R/future_map.R)                      |    65.22     |
| [R/global-gatherer.R](../R/global-gatherer.R)             |    65.98     |
| [R/future\_map\_template.R](../R/future_map_template.R)   |    80.00     |
| [R/future\_options.R](../R/future_options.R)              |    82.86     |
| [R/progress.R](../R/progress.R)                           |    90.91     |

<br>

## Unit Tests

Unit Test summary is created using the
[testthat](https://github.com/r-lib/testthat) package.

| file                                                    |  n |  time | error | failed | skipped | warning | icon |
| :------------------------------------------------------ | -: | ----: | ----: | -----: | ------: | ------: | :--- |
| [test-future-options.R](testthat/test-future-options.R) |  6 | 0.613 |     0 |      0 |       0 |       0 |      |
| [test-map.R](testthat/test-map.R)                       | 24 | 1.591 |     0 |      0 |       3 |       0 | 🔶    |
| [test-map2.R](testthat/test-map2.R)                     | 15 | 1.540 |     0 |      0 |       0 |       0 |      |
| [test-pmap.R](testthat/test-pmap.R)                     | 27 | 2.368 |     0 |      0 |       0 |       0 |      |
| [test-progress.R](testthat/test-progress.R)             |  4 | 6.339 |     0 |      0 |       0 |       0 |      |

<details open>

<summary> Show Detailed Test Results </summary>

| file                                                            | context               | test                                                                    | status  | n |  time | icon |
| :-------------------------------------------------------------- | :-------------------- | :---------------------------------------------------------------------- | :------ | -: | ----: | :--- |
| [test-future-options.R](testthat/test-future-options.R#L55_L56) | test-future-options.R | sequential - setting seed keeps reproducible numbers                    | PASS    | 1 | 0.026 |      |
| [test-future-options.R](testthat/test-future-options.R#L36)     | test-future-options.R | multisession - selective exporting of variables works                   | PASS    | 1 | 0.088 |      |
| [test-future-options.R](testthat/test-future-options.R#L42)     | test-future-options.R | multisession - selective exporting of packages works                    | PASS    | 2 | 0.398 |      |
| [test-future-options.R](testthat/test-future-options.R#L55_L56) | test-future-options.R | multisession - setting seed keeps reproducible numbers                  | PASS    | 1 | 0.053 |      |
| [test-future-options.R](testthat/test-future-options.R#L55_L56) | test-future-options.R | multicore - setting seed keeps reproducible numbers                     | PASS    | 1 | 0.048 |      |
| [test-map.R](testthat/test-map.R#L26)                           | test-map.R            | sequential - equivalence with map()                                     | PASS    | 1 | 0.025 |      |
| [test-map.R](testthat/test-map.R#L33)                           | test-map.R            | sequential - equivalence with vector map()s                             | PASS    | 1 | 0.012 |      |
| [test-map.R](testthat/test-map.R#L40)                           | test-map.R            | sequential - equivalence with df map()s                                 | PASS    | 1 | 0.016 |      |
| [test-map.R](testthat/test-map.R#L47)                           | test-map.R            | sequential - equivalence with map\_at()                                 | PASS    | 1 | 0.012 |      |
| [test-map.R](testthat/test-map.R#L54)                           | test-map.R            | sequential - equivalence with map\_if()                                 | PASS    | 1 | 0.011 |      |
| [test-map.R](testthat/test-map.R#L59)                           | test-map.R            | sequential - Working mutate+map double nest with \~                     | SKIPPED | 1 | 0.000 | 🔶    |
| [test-map.R](testthat/test-map.R#L92)                           | test-map.R            | sequential - Globals in .x are found (.x could be a fn)                 | PASS    | 1 | 0.015 |      |
| [test-map.R](testthat/test-map.R#L110)                          | test-map.R            | sequential - Globals in .x are only exported to workers that use them   | PASS    | 1 | 0.012 |      |
| [test-map.R](testthat/test-map.R#L26)                           | test-map.R            | multisession - equivalence with map()                                   | PASS    | 1 | 0.922 |      |
| [test-map.R](testthat/test-map.R#L33)                           | test-map.R            | multisession - equivalence with vector map()s                           | PASS    | 1 | 0.092 |      |
| [test-map.R](testthat/test-map.R#L40)                           | test-map.R            | multisession - equivalence with df map()s                               | PASS    | 1 | 0.147 |      |
| [test-map.R](testthat/test-map.R#L47)                           | test-map.R            | multisession - equivalence with map\_at()                               | PASS    | 1 | 0.025 |      |
| [test-map.R](testthat/test-map.R#L54)                           | test-map.R            | multisession - equivalence with map\_if()                               | PASS    | 1 | 0.024 |      |
| [test-map.R](testthat/test-map.R#L59)                           | test-map.R            | multisession - Working mutate+map double nest with \~                   | SKIPPED | 1 | 0.000 | 🔶    |
| [test-map.R](testthat/test-map.R#L92)                           | test-map.R            | multisession - Globals in .x are found (.x could be a fn)               | PASS    | 1 | 0.087 |      |
| [test-map.R](testthat/test-map.R#L110)                          | test-map.R            | multisession - Globals in .x are only exported to workers that use them | PASS    | 1 | 0.085 |      |
| [test-map.R](testthat/test-map.R#L26)                           | test-map.R            | multicore - equivalence with map()                                      | PASS    | 1 | 0.028 |      |
| [test-map.R](testthat/test-map.R#L33)                           | test-map.R            | multicore - equivalence with vector map()s                              | PASS    | 1 | 0.012 |      |
| [test-map.R](testthat/test-map.R#L40)                           | test-map.R            | multicore - equivalence with df map()s                                  | PASS    | 1 | 0.014 |      |
| [test-map.R](testthat/test-map.R#L47)                           | test-map.R            | multicore - equivalence with map\_at()                                  | PASS    | 1 | 0.011 |      |
| [test-map.R](testthat/test-map.R#L54)                           | test-map.R            | multicore - equivalence with map\_if()                                  | PASS    | 1 | 0.010 |      |
| [test-map.R](testthat/test-map.R#L59)                           | test-map.R            | multicore - Working mutate+map double nest with \~                      | SKIPPED | 1 | 0.001 | 🔶    |
| [test-map.R](testthat/test-map.R#L92)                           | test-map.R            | multicore - Globals in .x are found (.x could be a fn)                  | PASS    | 1 | 0.017 |      |
| [test-map.R](testthat/test-map.R#L110)                          | test-map.R            | multicore - Globals in .x are only exported to workers that use them    | PASS    | 1 | 0.013 |      |
| [test-map2.R](testthat/test-map2.R#L27)                         | test-map2.R           | sequential - equivalence with map2()                                    | PASS    | 1 | 0.010 |      |
| [test-map2.R](testthat/test-map2.R#L34)                         | test-map2.R           | sequential - equivalence with vector map2()s                            | PASS    | 1 | 0.090 |      |
| [test-map2.R](testthat/test-map2.R#L41)                         | test-map2.R           | sequential - equivalence with df map2()s                                | PASS    | 1 | 0.013 |      |
| [test-map2.R](testthat/test-map2.R#L56)                         | test-map2.R           | sequential - Globals in .x and .y are found (.y could be a fn)          | PASS    | 1 | 0.017 |      |
| [test-map2.R](testthat/test-map2.R#L64)                         | test-map2.R           | sequential - chunk balancing is correct after a .x recycle              | PASS    | 1 | 0.010 |      |
| [test-map2.R](testthat/test-map2.R#L27)                         | test-map2.R           | multisession - equivalence with map2()                                  | PASS    | 1 | 0.934 |      |
| [test-map2.R](testthat/test-map2.R#L34)                         | test-map2.R           | multisession - equivalence with vector map2()s                          | PASS    | 1 | 0.083 |      |
| [test-map2.R](testthat/test-map2.R#L41)                         | test-map2.R           | multisession - equivalence with df map2()s                              | PASS    | 1 | 0.151 |      |
| [test-map2.R](testthat/test-map2.R#L56)                         | test-map2.R           | multisession - Globals in .x and .y are found (.y could be a fn)        | PASS    | 1 | 0.057 |      |
| [test-map2.R](testthat/test-map2.R#L64)                         | test-map2.R           | multisession - chunk balancing is correct after a .x recycle            | PASS    | 1 | 0.093 |      |
| [test-map2.R](testthat/test-map2.R#L27)                         | test-map2.R           | multicore - equivalence with map2()                                     | PASS    | 1 | 0.030 |      |
| [test-map2.R](testthat/test-map2.R#L34)                         | test-map2.R           | multicore - equivalence with vector map2()s                             | PASS    | 1 | 0.010 |      |
| [test-map2.R](testthat/test-map2.R#L41)                         | test-map2.R           | multicore - equivalence with df map2()s                                 | PASS    | 1 | 0.013 |      |
| [test-map2.R](testthat/test-map2.R#L56)                         | test-map2.R           | multicore - Globals in .x and .y are found (.y could be a fn)           | PASS    | 1 | 0.018 |      |
| [test-map2.R](testthat/test-map2.R#L64)                         | test-map2.R           | multicore - chunk balancing is correct after a .x recycle               | PASS    | 1 | 0.011 |      |
| [test-pmap.R](testthat/test-pmap.R#L28)                         | test-pmap.R           | sequential - equivalence with pmap()                                    | PASS    | 1 | 0.011 |      |
| [test-pmap.R](testthat/test-pmap.R#L35)                         | test-pmap.R           | sequential - equivalence with vector pmap()s                            | PASS    | 1 | 0.094 |      |
| [test-pmap.R](testthat/test-pmap.R#L42)                         | test-pmap.R           | sequential - equivalence with df pmap()s                                | PASS    | 1 | 0.013 |      |
| [test-pmap.R](testthat/test-pmap.R#L57)                         | test-pmap.R           | sequential - named arguments can be passed through                      | PASS    | 1 | 0.011 |      |
| [test-pmap.R](testthat/test-pmap.R#L71)                         | test-pmap.R           | sequential - arguments can be matched by name                           | PASS    | 1 | 0.011 |      |
| [test-pmap.R](testthat/test-pmap.R#L82)                         | test-pmap.R           | sequential - unused components can be absorbed                          | PASS    | 2 | 0.022 |      |
| [test-pmap.R](testthat/test-pmap.R#L98)                         | test-pmap.R           | sequential - Globals in .l are found (.l could be a fn)                 | PASS    | 1 | 0.018 |      |
| [test-pmap.R](testthat/test-pmap.R#L117)                        | test-pmap.R           | sequential - Globals in .l are only exported to workers that use them   | PASS    | 1 | 0.012 |      |
| [test-pmap.R](testthat/test-pmap.R#L28)                         | test-pmap.R           | multisession - equivalence with pmap()                                  | PASS    | 1 | 0.953 |      |
| [test-pmap.R](testthat/test-pmap.R#L35)                         | test-pmap.R           | multisession - equivalence with vector pmap()s                          | PASS    | 1 | 0.083 |      |
| [test-pmap.R](testthat/test-pmap.R#L42)                         | test-pmap.R           | multisession - equivalence with df pmap()s                              | PASS    | 1 | 0.153 |      |
| [test-pmap.R](testthat/test-pmap.R#L57)                         | test-pmap.R           | multisession - named arguments can be passed through                    | PASS    | 1 | 0.096 |      |
| [test-pmap.R](testthat/test-pmap.R#L71)                         | test-pmap.R           | multisession - arguments can be matched by name                         | PASS    | 1 | 0.086 |      |
| [test-pmap.R](testthat/test-pmap.R#L82)                         | test-pmap.R           | multisession - unused components can be absorbed                        | PASS    | 2 | 0.248 |      |
| [test-pmap.R](testthat/test-pmap.R#L98)                         | test-pmap.R           | multisession - Globals in .l are found (.l could be a fn)               | PASS    | 1 | 0.361 |      |
| [test-pmap.R](testthat/test-pmap.R#L117)                        | test-pmap.R           | multisession - Globals in .l are only exported to workers that use them | PASS    | 1 | 0.050 |      |
| [test-pmap.R](testthat/test-pmap.R#L28)                         | test-pmap.R           | multicore - equivalence with pmap()                                     | PASS    | 1 | 0.032 |      |
| [test-pmap.R](testthat/test-pmap.R#L35)                         | test-pmap.R           | multicore - equivalence with vector pmap()s                             | PASS    | 1 | 0.012 |      |
| [test-pmap.R](testthat/test-pmap.R#L42)                         | test-pmap.R           | multicore - equivalence with df pmap()s                                 | PASS    | 1 | 0.015 |      |
| [test-pmap.R](testthat/test-pmap.R#L57)                         | test-pmap.R           | multicore - named arguments can be passed through                       | PASS    | 1 | 0.012 |      |
| [test-pmap.R](testthat/test-pmap.R#L71)                         | test-pmap.R           | multicore - arguments can be matched by name                            | PASS    | 1 | 0.011 |      |
| [test-pmap.R](testthat/test-pmap.R#L82)                         | test-pmap.R           | multicore - unused components can be absorbed                           | PASS    | 2 | 0.023 |      |
| [test-pmap.R](testthat/test-pmap.R#L98)                         | test-pmap.R           | multicore - Globals in .l are found (.l could be a fn)                  | PASS    | 1 | 0.028 |      |
| [test-pmap.R](testthat/test-pmap.R#L117)                        | test-pmap.R           | multicore - Globals in .l are only exported to workers that use them    | PASS    | 1 | 0.013 |      |
| [test-progress.R](testthat/test-progress.R#L32)                 | test-progress.R       | multisession - Progress bar is emitted on long running tasks            | PASS    | 1 | 3.517 |      |
| [test-progress.R](testthat/test-progress.R#L40)                 | test-progress.R       | multisession - Progress bar is not emitted on short running tasks       | PASS    | 1 | 0.093 |      |
| [test-progress.R](testthat/test-progress.R#L32)                 | test-progress.R       | multicore - Progress bar is emitted on long running tasks               | PASS    | 1 | 2.619 |      |
| [test-progress.R](testthat/test-progress.R#L40)                 | test-progress.R       | multicore - Progress bar is not emitted on short running tasks          | PASS    | 1 | 0.110 |      |

| Failed | Warning | Skipped |
| :----- | :------ | :------ |
| 🛑      | ⚠️      | 🔶       |

</details>

<details>

<summary> Session Info </summary>

| Field    | Value                               |
| :------- | :---------------------------------- |
| Version  | R version 3.6.1 (2019-07-05)        |
| Platform | x86\_64-apple-darwin15.6.0 (64-bit) |
| Running  | macOS Mojave 10.14.5                |
| Language | en\_US                              |
| Timezone | America/New\_York                   |

| Package  | Version |
| :------- | :------ |
| testthat | 2.2.1   |
| covr     | 3.3.0   |
| covrpage | 0.0.70  |

</details>

<!--- Final Status : skipped/warning --->
