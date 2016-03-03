# Deep Learning Benchmarks

## Introduction

This repository contains structured performance characteristics of the
most popular Machine and Deep Learning Frameworks forward and backward
performance for entire models, single layers and more. Deep Learning Benchmarks
is inspired by soumith's [convnet-benchmarks][convnet-benchmarks] and zer0n's
[deepframeworks][deepframeworks].

`Deep Learning Benchmarks` goal is to provide raw, structured, comparable data
about the performance (operational speed, operational memory usage) of different
Machine Learning Frameworks in various environments and machines. Like the other
two repositories, `Deep Learning Benchmarks` highest goal is gaining objective,
reproducible benchmarks, which are reviewed by the community. New benchmark data is
introduced through PRs, its process is described in
[Submitting Benchmark Date][submitting-benchmark-data].

One advantage of structured, raw benchmark data is, that it can be easily
queried, visualized and compared.
[Autumn's Benchmark page][autumn-benchmark-page], provides an open interface for
querying and visualizing the Deep Learning Benchmark data.

[convnet-benchmarks]: https://github.com/soumith/convnet-benchmarks
[deepframeworks]: https://github.com/zer0n/deepframeworks
[submitting-benchmark-data]: #submitting-benchmark-data
[autumn-benchmark-page]: http://autumnai.com

## Data

The repository contains this [README](README.md) and
[benchmark.toml](benchmark.toml), where all the benchmark data is stored.

You can consume the data like a JSON REST-API, by fetching

```
https://raw.githubusercontent.com/autumnai/deep-learning-benchmarks/master/benchmark.json
```

```javascript
fetch('https://raw.githubusercontent.com/autumnai/deep-learning-benchmarks/master/benchmark.json')
  .then(function(response) {
    return response.json()
  }).then(function(json) {
    console.log('parsed json', json)
  }).catch(function(ex) {
    console.log('parsing failed', ex)
  })
```

We use TOML for the original benchmark data file format (instead of JSON),
because it is more convenient for merging data. Out of convenience we convert
the TOML into a JSON file locally as well before we merge a PR, this increases
the usability of the data for client-side applications.

## Data Structure

> WIP

## Submitting Benchmark Data

> WIP
