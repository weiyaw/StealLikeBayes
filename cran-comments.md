## R CMD check results

- running `devtools::check(remote = TRUE, manual = TRUE)` gives no errors, warnings, and 1 note:
```
❯ checking CRAN incoming feasibility ... [4s/58s] NOTE
  Maintainer: ‘Tomasz Woźniak <wozniak.tom@pm.me>’
  
  New submission
```
We are happy about it.

- running `devtools::check_win_devel()` returns gives no errors, warnings, and 1 note:
```
* checking CRAN incoming feasibility ... NOTE
Maintainer: 'Tomasz Woźniak <wozniak.tom@pm.me>'

New submission

Possibly misspelled words in DESCRIPTION:
  repurpose (61:28)
```
We are happy about it too.

- the package passes all the checks on GH action from the standard setup `R-CMD-check.yaml`

- the package passes all procedures following `usethis::use_release_issue()`