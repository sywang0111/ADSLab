---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: ISM- An Intra-Stripe Data Migration Approach for RAID-5 Scaling
subtitle: ''
summary: ''
authors:
- Jie Liang
- Yinlong Xu
- Yongkun Li
- Yubiao Pan
tags:
- '"Arrays"'
- '"Bandwidth"'
- '"coding relationship"'
- '"Computer science"'
- '"data blocks"'
- '"data handling"'
- '"DiskSim"'
- '"High performance computing"'
- '"I/O performance"'
- '"intra-stripe data migration"'
- '"ISM"'
- '"Layout"'
- '"Parallel processing"'
- '"parity blocks"'
- '"RAID"'
- '"RAID-5 scaling"'
- '"RAID-5 system"'
- '"redundant array of inexpensive disks"'
- '"storage capacity"'
- '"storage management"'
- '"Strips"'
categories: []
date: '2017-08-01'
lastmod: 2020-10-16T11:09:12+08:00
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
publishDate: '2020-10-16T03:09:12.190229Z'
publication_types:
- '1'
abstract: 'Scaling is often carried out in modern RAID systems to meet the ever increasing
  demand of storage capacity and I/O performance. However, the scaling process of
  RAID-5 system is not trivial, due to its specific data/parity layout. Previous approaches
  of RAID-5 scaling require either migrating almost all data blocks in the system,
  or recalculating all or some of the parity blocks during scaling. This paper proposes
  a new RAID-5 scaling approach called ISM (Intra-Stripe Migration). With ISM, data
  migrations only happen within stripes, which means that the coding relationship
  among blocks remains the same. Therefore, the parity blocks do not need to be recalculated
  after data migration, which greatly reduces the I/O and computational costs. The
  properties of ISM approach can be summarized as follows: (1) it requires the minimum
  amount of data blocks to be migrated, (2) it supports data migration without recalculating
  parity blocks, and (3) it supports multiple successive scaling operations while
  keeping the above properties. The simulation results on DiskSim show that: (1) ISM
  reduces the scaling time from 47.91% to 87.01% and from 88.94% to 96.58% compared
  with GSR and ALV respectively in offline scaling, (2) under two real-world I/O traces,
  ISM also outperforms GSR by 64.15% to 87.30%, and ALV by 92.38% to 95.98% in scaling
  time, and (3) ISM maintains almost the same performance of data access with ALV
  and GSR after scaling.'
publication: '*2017 International Conference on Networking, Architecture, and Storage
  (NAS)*'
doi: 10.1109/NAS.2017.8026863
---
