---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: 'BiloKey : A Scalable Bi-Index Locality-Aware In-Memory Key-Value Store'
subtitle: ''
summary: ''
authors:
- Wenlong Ma
- Yuqing Zhu
- Cheng Li
- Mengying Guo
- Yungang Bao
tags:
- '"bi-index locality-aware"'
- '"BiloKey"'
- '"cache storage"'
- '"Complexity theory"'
- '"computational complexity"'
- '"Concurrency control"'
- '"data structures"'
- '"Data structures"'
- '"fast in-memory key value stores"'
- '"fast in-memory KV stores"'
- '"hash table index"'
- '"hybrid index"'
- '"In-memory key-value store"'
- '"Indexing"'
- '"Instruction sets"'
- '"Internet"'
- '"Internet services"'
- '"lazy synchronization"'
- '"locality-aware data parallel processing"'
- '"locality-aware networking"'
- '"lock-free access"'
- '"lock-free data structure"'
- '"Memcached"'
- '"multi-core scalability"'
- '"multicore machines"'
- '"multiprocessing systems"'
- '"parallel processing"'
- '"read-intensive workloads"'
- '"Redis"'
- '"Scalability"'
- '"scan-intensive workloads"'
- '"skiplist index"'
- '"storage management"'
- '"synchronisation"'
- '"write-intensive workloads"'
categories: []
date: '2019-07-01'
lastmod: 2020-10-16T11:09:25+08:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
publishDate: '2020-10-16T03:09:24.825368Z'
publication_types:
- '2'
abstract: 'Fast in-memory key value stores are the keys to building large-scale Internet
  services. The state-of-the-art solutions mainly focus on optimizing the performance
  for read-intensive workloads. Nevertheless, a wide range of applications demonstrate
  a significant amount of updates and range queries, which scale poorly with the current
  implementations. In this paper, we present BiloKey, a highly scalable in-memory
  key value store on multi-core machines, significantly outperforming Redis and Memcached
  for a variety of mixed read and write workloads. To achieve this, BiloKey leverages
  a fast bi-index comprised by a Hash Table index and a SkipList index, where the
  former supports feature rich operations including GET, UPDATE and DELETE with O(1)
  complexity, while the latter supports SCAN with O(log N) complexity. Furthermore,
  to make the bi-index design scale well, BiloKey adopts three techniques: lazy synchronization
  for reducing the overhead of maintaining index consistency, lock-free data structure
  for supporting multi-writers, and locality-aware data parallel processing for preserving
  the data locality of requests. Compared with two popular in-memory KV stores (i.e.,
  Redis and Memcached), experimental results show that: (1) for write-intensive workloads,
  BiloKey outperforms Redis and Memcached by 7.8x and 3.7x on average (up to 11.5x
  and 4.8x), respectively; (2) for scan-intensive workloads, BiloKey achieves an average
  speedup of 2.3x against Redis; (3) for read-intensive workloads, BiloKey also outperforms
  Redis and Memcached by 1.2x and 1.8x on average.'
publication: '*IEEE Transactions on Parallel and Distributed Systems*'
doi: 10.1109/TPDS.2019.2891599
---
