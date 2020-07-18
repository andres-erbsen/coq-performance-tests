# coq-performance-tests
[![CI (Coq)](https://github.com/coq-community/coq-performance-tests/workflows/CI%20(Coq)/badge.svg)](https://github.com/coq-community/coq-performance-tests/actions?query=branch%3Amaster+workflow%3A%22CI+%28Coq%29%22)

A library of Coq source files testing for performance regressions on Coq

## Contributing

Please add tests to this repository.

Each test should go in its own .v file in [`src/`](./src/), and each .v file should be
targeted to take around 1 minute, so that all tests get roughly equal
weight.

## PerformanceExperiments

The [`PerformanceExperiments`](./PerformanceExperiments/) folder contains a number of tests based on a [test harness file](./PerformanceExperiments/Harness.v) which allow automatic generation of plots, as displayed below.
The plots are updated on each run of GitHub Actions.
To contribute to this folder, please add your test to [`Makefile.variables.kinds`](./PerformanceExperiments/Makefile.variables.kinds) and follow the format of the existing tests.
You can use `make update-README` to regenerate the tables for this README.

### PerformanceExperiments plots

- [`pattern`](./PerformanceExperiments/pattern.v)

  master | 8.11.2 | 8.10.2 | 8.9.1 | 8.8.2
  --|--|--|--|--
  <a href="https://coq-community.github.io/coq-performance-tests/master/pattern.svg">"<img src="https://coq-community.github.io/coq-performance-tests/master/pattern.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.11.2/pattern.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.11.2/pattern.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.10.2/pattern.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.10.2/pattern.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.9.1/pattern.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.9.1/pattern.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.8.2/pattern.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.8.2/pattern.svg" height=100px /></a>

- [`n_polymorphic_universes`](./PerformanceExperiments/n_polymorphic_universes.v)

  master | 8.11.2 | 8.10.2 | 8.9.1 | 8.8.2
  --|--|--|--|--
  <a href="https://coq-community.github.io/coq-performance-tests/master/n-polymorphic-universes.svg">"<img src="https://coq-community.github.io/coq-performance-tests/master/n-polymorphic-universes.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.11.2/n-polymorphic-universes.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.11.2/n-polymorphic-universes.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.10.2/n-polymorphic-universes.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.10.2/n-polymorphic-universes.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.9.1/n-polymorphic-universes.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.9.1/n-polymorphic-universes.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.8.2/n-polymorphic-universes.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.8.2/n-polymorphic-universes.svg" height=100px /></a>

- [`repeat_setoid_rewrite_under_binders`](./PerformanceExperiments/repeat_setoid_rewrite_under_binders.v)

  master | 8.11.2 | 8.10.2 | 8.9.1 | 8.8.2
  --|--|--|--|--
  <a href="https://coq-community.github.io/coq-performance-tests/master/repeat-setoid-rewrite-under-binders.svg">"<img src="https://coq-community.github.io/coq-performance-tests/master/repeat-setoid-rewrite-under-binders.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.11.2/repeat-setoid-rewrite-under-binders.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.11.2/repeat-setoid-rewrite-under-binders.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.10.2/repeat-setoid-rewrite-under-binders.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.10.2/repeat-setoid-rewrite-under-binders.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.9.1/repeat-setoid-rewrite-under-binders.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.9.1/repeat-setoid-rewrite-under-binders.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.8.2/repeat-setoid-rewrite-under-binders.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.8.2/repeat-setoid-rewrite-under-binders.svg" height=100px /></a>

- [`repeat_setoid_rewrite_under_binders_noop`](./PerformanceExperiments/repeat_setoid_rewrite_under_binders_noop.v)

  master | 8.11.2 | 8.10.2 | 8.9.1 | 8.8.2
  --|--|--|--|--
  <a href="https://coq-community.github.io/coq-performance-tests/master/repeat-setoid-rewrite-under-binders-noop.svg">"<img src="https://coq-community.github.io/coq-performance-tests/master/repeat-setoid-rewrite-under-binders-noop.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.11.2/repeat-setoid-rewrite-under-binders-noop.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.11.2/repeat-setoid-rewrite-under-binders-noop.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.10.2/repeat-setoid-rewrite-under-binders-noop.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.10.2/repeat-setoid-rewrite-under-binders-noop.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.9.1/repeat-setoid-rewrite-under-binders-noop.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.9.1/repeat-setoid-rewrite-under-binders-noop.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.8.2/repeat-setoid-rewrite-under-binders-noop.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.8.2/repeat-setoid-rewrite-under-binders-noop.svg" height=100px /></a>

- [`rewrite_strat_under_binders`](./PerformanceExperiments/rewrite_strat_under_binders.v)

  master | 8.11.2 | 8.10.2 | 8.9.1 | 8.8.2
  --|--|--|--|--
  <a href="https://coq-community.github.io/coq-performance-tests/master/rewrite-strat-under-binders.svg">"<img src="https://coq-community.github.io/coq-performance-tests/master/rewrite-strat-under-binders.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.11.2/rewrite-strat-under-binders.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.11.2/rewrite-strat-under-binders.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.10.2/rewrite-strat-under-binders.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.10.2/rewrite-strat-under-binders.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.9.1/rewrite-strat-under-binders.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.9.1/rewrite-strat-under-binders.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.8.2/rewrite-strat-under-binders.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.8.2/rewrite-strat-under-binders.svg" height=100px /></a>

- [`rewrite_repeated_app_autorewrite`](./PerformanceExperiments/rewrite_repeated_app_autorewrite.v)

  master | 8.11.2 | 8.10.2 | 8.9.1 | 8.8.2
  --|--|--|--|--
  <a href="https://coq-community.github.io/coq-performance-tests/master/rewrite-repeated-app-autorewrite.svg">"<img src="https://coq-community.github.io/coq-performance-tests/master/rewrite-repeated-app-autorewrite.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.11.2/rewrite-repeated-app-autorewrite.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.11.2/rewrite-repeated-app-autorewrite.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.10.2/rewrite-repeated-app-autorewrite.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.10.2/rewrite-repeated-app-autorewrite.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.9.1/rewrite-repeated-app-autorewrite.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.9.1/rewrite-repeated-app-autorewrite.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.8.2/rewrite-repeated-app-autorewrite.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.8.2/rewrite-repeated-app-autorewrite.svg" height=100px /></a>

- [`rewrite_repeated_app_autorewrite_noop`](./PerformanceExperiments/rewrite_repeated_app_autorewrite_noop.v)

  master | 8.11.2 | 8.10.2 | 8.9.1 | 8.8.2
  --|--|--|--|--
  <a href="https://coq-community.github.io/coq-performance-tests/master/rewrite-repeated-app-autorewrite-noop.svg">"<img src="https://coq-community.github.io/coq-performance-tests/master/rewrite-repeated-app-autorewrite-noop.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.11.2/rewrite-repeated-app-autorewrite-noop.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.11.2/rewrite-repeated-app-autorewrite-noop.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.10.2/rewrite-repeated-app-autorewrite-noop.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.10.2/rewrite-repeated-app-autorewrite-noop.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.9.1/rewrite-repeated-app-autorewrite-noop.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.9.1/rewrite-repeated-app-autorewrite-noop.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.8.2/rewrite-repeated-app-autorewrite-noop.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.8.2/rewrite-repeated-app-autorewrite-noop.svg" height=100px /></a>

- [`rewrite_repeated_app_ssrrewrite`](./PerformanceExperiments/rewrite_repeated_app_ssrrewrite.v)

  master | 8.11.2 | 8.10.2 | 8.9.1 | 8.8.2
  --|--|--|--|--
  <a href="https://coq-community.github.io/coq-performance-tests/master/rewrite-repeated-app-ssrrewrite.svg">"<img src="https://coq-community.github.io/coq-performance-tests/master/rewrite-repeated-app-ssrrewrite.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.11.2/rewrite-repeated-app-ssrrewrite.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.11.2/rewrite-repeated-app-ssrrewrite.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.10.2/rewrite-repeated-app-ssrrewrite.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.10.2/rewrite-repeated-app-ssrrewrite.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.9.1/rewrite-repeated-app-ssrrewrite.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.9.1/rewrite-repeated-app-ssrrewrite.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.8.2/rewrite-repeated-app-ssrrewrite.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.8.2/rewrite-repeated-app-ssrrewrite.svg" height=100px /></a>

- [`rewrite_repeated_app_ssrrewrite_noop`](./PerformanceExperiments/rewrite_repeated_app_ssrrewrite_noop.v)

  master | 8.11.2 | 8.10.2 | 8.9.1 | 8.8.2
  --|--|--|--|--
  <a href="https://coq-community.github.io/coq-performance-tests/master/rewrite-repeated-app-ssrrewrite-noop.svg">"<img src="https://coq-community.github.io/coq-performance-tests/master/rewrite-repeated-app-ssrrewrite-noop.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.11.2/rewrite-repeated-app-ssrrewrite-noop.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.11.2/rewrite-repeated-app-ssrrewrite-noop.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.10.2/rewrite-repeated-app-ssrrewrite-noop.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.10.2/rewrite-repeated-app-ssrrewrite-noop.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.9.1/rewrite-repeated-app-ssrrewrite-noop.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.9.1/rewrite-repeated-app-ssrrewrite-noop.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.8.2/rewrite-repeated-app-ssrrewrite-noop.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.8.2/rewrite-repeated-app-ssrrewrite-noop.svg" height=100px /></a>

- [`rewrite_repeated_app_rewrite_strat`](./PerformanceExperiments/rewrite_repeated_app_rewrite_strat.v)

  master | 8.11.2 | 8.10.2 | 8.9.1 | 8.8.2
  --|--|--|--|--
  <a href="https://coq-community.github.io/coq-performance-tests/master/rewrite-repeated-app-rewrite-strat.svg">"<img src="https://coq-community.github.io/coq-performance-tests/master/rewrite-repeated-app-rewrite-strat.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.11.2/rewrite-repeated-app-rewrite-strat.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.11.2/rewrite-repeated-app-rewrite-strat.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.10.2/rewrite-repeated-app-rewrite-strat.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.10.2/rewrite-repeated-app-rewrite-strat.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.9.1/rewrite-repeated-app-rewrite-strat.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.9.1/rewrite-repeated-app-rewrite-strat.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.8.2/rewrite-repeated-app-rewrite-strat.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.8.2/rewrite-repeated-app-rewrite-strat.svg" height=100px /></a>

- [`rewrite_repeated_app_fast_rewrite`](./PerformanceExperiments/rewrite_repeated_app_fast_rewrite.v)

  master | 8.11.2 | 8.10.2 | 8.9.1 | 8.8.2
  --|--|--|--|--
  <a href="https://coq-community.github.io/coq-performance-tests/master/rewrite-repeated-app-fast-rewrite.svg">"<img src="https://coq-community.github.io/coq-performance-tests/master/rewrite-repeated-app-fast-rewrite.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.11.2/rewrite-repeated-app-fast-rewrite.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.11.2/rewrite-repeated-app-fast-rewrite.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.10.2/rewrite-repeated-app-fast-rewrite.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.10.2/rewrite-repeated-app-fast-rewrite.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.9.1/rewrite-repeated-app-fast-rewrite.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.9.1/rewrite-repeated-app-fast-rewrite.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.8.2/rewrite-repeated-app-fast-rewrite.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.8.2/rewrite-repeated-app-fast-rewrite.svg" height=100px /></a>

- [`rewrite_repeated_app_fast_rewrite_no_abstract`](./PerformanceExperiments/rewrite_repeated_app_fast_rewrite_no_abstract.v)

  master | 8.11.2 | 8.10.2 | 8.9.1 | 8.8.2
  --|--|--|--|--
  <a href="https://coq-community.github.io/coq-performance-tests/master/rewrite-repeated-app-fast-rewrite-no-abstract.svg">"<img src="https://coq-community.github.io/coq-performance-tests/master/rewrite-repeated-app-fast-rewrite-no-abstract.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.11.2/rewrite-repeated-app-fast-rewrite-no-abstract.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.11.2/rewrite-repeated-app-fast-rewrite-no-abstract.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.10.2/rewrite-repeated-app-fast-rewrite-no-abstract.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.10.2/rewrite-repeated-app-fast-rewrite-no-abstract.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.9.1/rewrite-repeated-app-fast-rewrite-no-abstract.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.9.1/rewrite-repeated-app-fast-rewrite-no-abstract.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.8.2/rewrite-repeated-app-fast-rewrite-no-abstract.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.8.2/rewrite-repeated-app-fast-rewrite-no-abstract.svg" height=100px /></a>

- [`typeclass_reification_let_in_HOAS`](./PerformanceExperiments/typeclass_reification_let_in_HOAS.v)

  master | 8.11.2 | 8.10.2 | 8.9.1 | 8.8.2
  --|--|--|--|--
  <a href="https://coq-community.github.io/coq-performance-tests/master/typeclass-reification-let-in-HOAS.svg">"<img src="https://coq-community.github.io/coq-performance-tests/master/typeclass-reification-let-in-HOAS.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.11.2/typeclass-reification-let-in-HOAS.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.11.2/typeclass-reification-let-in-HOAS.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.10.2/typeclass-reification-let-in-HOAS.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.10.2/typeclass-reification-let-in-HOAS.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.9.1/typeclass-reification-let-in-HOAS.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.9.1/typeclass-reification-let-in-HOAS.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.8.2/typeclass-reification-let-in-HOAS.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.8.2/typeclass-reification-let-in-HOAS.svg" height=100px /></a>

- [`typeclass_reification_let_in_PHOAS`](./PerformanceExperiments/typeclass_reification_let_in_PHOAS.v)

  master | 8.11.2 | 8.10.2 | 8.9.1 | 8.8.2
  --|--|--|--|--
  <a href="https://coq-community.github.io/coq-performance-tests/master/typeclass-reification-let-in-PHOAS.svg">"<img src="https://coq-community.github.io/coq-performance-tests/master/typeclass-reification-let-in-PHOAS.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.11.2/typeclass-reification-let-in-PHOAS.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.11.2/typeclass-reification-let-in-PHOAS.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.10.2/typeclass-reification-let-in-PHOAS.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.10.2/typeclass-reification-let-in-PHOAS.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.9.1/typeclass-reification-let-in-PHOAS.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.9.1/typeclass-reification-let-in-PHOAS.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.8.2/typeclass-reification-let-in-PHOAS.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.8.2/typeclass-reification-let-in-PHOAS.svg" height=100px /></a>

- [`rewrite_repeated_app_fast_rewrite_ltac2`](./PerformanceExperiments/rewrite_repeated_app_fast_rewrite_ltac2.v)

  master | 8.11.2 | 8.10.2 | 8.9.1 | 8.8.2
  --|--|--|--|--
  <a href="https://coq-community.github.io/coq-performance-tests/master/rewrite-repeated-app-fast-rewrite-ltac2.svg">"<img src="https://coq-community.github.io/coq-performance-tests/master/rewrite-repeated-app-fast-rewrite-ltac2.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.11.2/rewrite-repeated-app-fast-rewrite-ltac2.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.11.2/rewrite-repeated-app-fast-rewrite-ltac2.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.10.2/rewrite-repeated-app-fast-rewrite-ltac2.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.10.2/rewrite-repeated-app-fast-rewrite-ltac2.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.9.1/rewrite-repeated-app-fast-rewrite-ltac2.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.9.1/rewrite-repeated-app-fast-rewrite-ltac2.svg" height=100px /></a> | <a href="https://coq-community.github.io/coq-performance-tests/8.8.2/rewrite-repeated-app-fast-rewrite-ltac2.svg">"<img src="https://coq-community.github.io/coq-performance-tests/8.8.2/rewrite-repeated-app-fast-rewrite-ltac2.svg" height=100px /></a>
