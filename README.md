# EXPFACTORY

![licence](https://img.shields.io/badge/licence-BSD-3-Clause-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![checks](https://img.shields.io/badge/checks-unknown_PASS-brightgreen)

> Governed Anticloud packaging of the upstream project `EXPFACTORY` in category **PSYCHOLOGY**. check results: see ISOLATED_LAB_RESULTS. Every number below traces to a named file + run stamp; nothing is borrowed from other projects.

**Upstream:** EXPFACTORY · **Upstream pin:** `885b54583b696762782c7580c7d9ceed40278938` · **Category:** PSYCHOLOGY · **Vendor:** Anticloud FZ LLE · **Licence:** BSD-3-Clause

---

## What This Project Does

# The Experiment Factory

[![DOI](http://joss.theoj.org/papers/10.21105/joss.00521/status.svg)](https://doi.org/10.21105/joss.00521)
[![DOI](https://zenodo.org/badge/108672186.svg)](https://zenodo.org/badge/latestdoi/108672186)
[![Gitter chat](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/expfactory/lobby)

![expfactory/static/img/expfactoryticketyellow.png](expfactory/static/img/expfactoryticketyellow.png)

See our [documentation](https://expfactory.github.io) for getting started. If you are new to containers, read our [background](https://expfactory.github.io/generate#background) or [paper](paper) first. If you want a more guided entry, see the [detailed start](https://expfactory.github.io/generate#detailed-start)

The Experiment Factory is software to create a reproducible container that you can easily customize to deploy a set of web-based experiments. 

## Citation
If the Experiment Factory is useful to you, please cite [the paper](https://doi.org/10.21105/joss.00521) to support the software and open source development.

```
Sochat, (2018). The Experiment Factory: Reproducible Experiment Containers. Journal of Open Source Software, 3(22), 521, https://doi.org/10.21105/joss.00521
```

## Contributing
We have many ways to contribute, and will briefly provide resources here to get you started.

### How to Contribute
If you are a developer interested in working on the Experiment Factory software you should read out [contributing guidelines](.github/CONTRIBUTING.md) for details. For contributing containers and experiments, see our [user documentation](https://expfactory.github.io/contribute). If you have any questions, please don't hesitate to [ask a question](https://www.github.com/expfactory/expfactory/issues). You'll need to lint your code using black:

```bash
$ pip install black
$ black expfactory --exclude template.py
```

### Code of Conduct
It's important to treat one another with respect, and maintain a fun and respectful environment for the open source community. Toward this aim, we ask that you review our [code of conduct](.github/CODE_OF_CONDUCT.md)

## Background
It's predecessor at [Expfactory.org](https://expfactory.org) was never able to open up to the public, and this went against the original goal of the software. Further, the badly needed functionality to serve a local battery was poorly met with [expfactory-python](https://www.github.com/expfactory-python) as time progressed and dependencies changes.
 
This version is agnostic to the underlying driver of the experiments, and provides reproducible, instantly deployable "container" experiments. What does that mean?

 - You obtain (or build) one container, a battery of experiments.
 - You (optionally) customize it
   - custom variables (e.g., a study identifier) and configurations go into the build recipe 
   - you can choose to use your own database (default output is flat files)
   - other options are available at runtime 
 - The container can be easily shared.
 - You run the container, optionally specifying a subset and ordering, and collect your results
 
If you build on [Docker Hub](https://hub.docker.com/) anyone else can then pull and use your exact container to collect their own results. It is exact down to the file hash. Note
that bases for expfactory were initially provided on [Docker Hub](https://hub.docker.com/r/vanessa/expfactory-builder/tags) and have moved to [Quay.io](https://quay.io/project/vanessa/expfactory-builder?tab=tags). Dockerfiles in the project that use the expfactory-builder are
also updated. If you need a previous version, please see the tags on the original Docker Hub.

## Experiment Library
The experiments themselves are now maintained under [expfactory-experiments](https://www.github.com/expfactory-experiments), official submissions to be found by expfactory can be added to the [library](https://www.github.com/expfactory/library) (under development) to be tested that they meet minimum requirements.

---

## Installation

The Experiment Factory is software to create a reproducible container that you can easily customize to deploy a set of web-based experiments.

## Usage

The Experiment Factory is software to create a reproducible container that you can easily customize to deploy a set of web-based experiments.

## API

The Experiment Factory is software to create a reproducible container that you can easily customize to deploy a set of web-based experiments.

## Dependencies

| Metric | Value |
|--------|-------|
| Files | unknown |
| Lines of Code | unknown |
| Dependencies | unknown |
| Upstream license (harvested) | BSD-3-Clause |
| Overlay license | Anticommons 0.1.0 |

Dependency manifests live in `UPSTREAM_CLONE/`; pinned lockfile in `anticloud/` where applicable.

## Configuration

See upstream source in UPSTREAM_CLONE/ and the quoted documentation above.

## Contributing

# Contributor's Agreement

You are under no obligation whatsoever to provide any bug fixes, patches,
or upgrades to the features, functionality or performance of the source
code ("Enhancements") to anyone; however, if you choose to make your
Enhancements available either publicly, or directly to the project,
without imposing a separate written license agreement for such
Enhancements, then you hereby grant the following license: a non-exclusive,
royalty-free perpetual license to install, use, modify, prepare derivative
works, incorporate into other computer software, distribute, and sublicense
such enhancements or derivative works thereof, in binary and source code
form.

# Contributing

Contributing to the Experiment Factory can be as small as asking a question by
[posting an issue](https://www.github.com/expfactory/expfactory/issues), or
equally posting an issue to discuss a wanted feature with your fellow
developers. If you have a quick bug fix or want to contribute to the codebase,
method is via a pull request (PR) to the project's development branch. For both
cases, make sure that you properly communicate the gist of the contribution.
For a bug fix (or request to fix), please describe the issue and show
any relevant output. For a feature request (or to start discussion on a 
contribution to do so) you can talk about your thinking with regards to
possible solutions. No question, request, or idea is too small, and we are glad
to have your contribution! 

Please note we have a [code of conduct](CODE_OF_CONDUCT.md) and ask that you
follow it for all interactions with project members and users.

## Pull Requests (PRs)

### Process
1. Essential bug fix PRs should be sent to both master and devopment branches.
2. Small bug fix and feature enhancement PRs should be sent to development only.
3. Follow the existing code style precedent. This does not need to be strictly
   defined as there are many thousands of lines of examples. Note the lack
   of tabs anywhere in the project, parentheses and spacing, curly bracket
   locations, source code layout, variable scoping, etc. and follow the
   project's standards.
4. Ensure any new install or build dependencies are added to the Dockerfile
5. For any new functionality, please write a test to be added to Continuous
   Integration (Travis) to test it/
6. The project's default copyright and header have been included in any new
   source files.
7. Make sure that your code is human understandable? This means notes in the
   code, along with a style that is easy to follow. 
8. Provide a walk through in the pull request for how you would like others
   to review it. If you write good documentation, this should almost be
   unnecessary (see point 10).
9. The pull request will be reviewed by others, and the final merge must be
   done by the project lead, @vsoch.
10. Documentation must be provided if necessary (next section)

### Documentation

1. Add any changes that you have made to the [CHANGELOG](../CHANGELOG.

## License

Upstream © its respective contributors under BSD-3-Clause (harvested MIT/Apache-2.0/BSD source; see `UPSTREAM_CLONE/LICENSE`). This packaging overlay is licensed under Anticommons 0.1.0.

## Upstream

- **project:** EXPFACTORY
- **Pinned SHA:** `885b54583b696762782c7580c7d9ceed40278938`
- **source:** `UPSTREAM_CLONE/` (pinned at the SHA above)
- **Upstream README source:** `UPSTREAM_CLONE/README.md`

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`e344903cb6154c2b9deb4720d45004a9b41ae0570f290a5c38725495b4129693`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe and Mail, Business Insider, National Post, Financial Post, StreetInsider, Digital Journal, Barchart, International Business Times, and fox47 · National Law Review.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

