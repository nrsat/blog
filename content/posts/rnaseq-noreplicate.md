---
categories:
- R
date: "2021-02-04"
draft: false
title: RNA-Seq without replication
---

### Replicateの無いRNA-SeqでDESeq2を使うには

ここが参考になった（[Bioconductor](https://support.bioconductor.org/p/119731/)）。

> “I’d recommend that you compute the vst() of the dataset and look at
> the large LFCs (difference between the two VST samples). I don’t think
> the pvalues were useful at all, hence the deprecation. I think the
> best we can do is output shrunken LFC (which here you can get by
> looking at difference between VST samples).”

昔は1サンプルをReplicateとして取り扱うことが出来たらしいが、上記の通り統計学的な意味が無くDeprecateとなったらしい。
