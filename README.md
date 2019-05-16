# Data to Cloud Tutorials

## Overview

This repository contains a collections of tutorials that aim to provide data-to-cloud technologies and hands-on tutorials for different environment and scenarios, and each gives the step-by-step guideline for customers to build a data-to-cloud process.

This series is not telling customer how to migrate the data from their on-premises environment to cloud at once, for example some companies need to change their OLTP database from Oracle to Mysql etc. However, the series is providing a practical way for companies/governments/organizations to build up a data tunnel for extracting data from operational source systems to Alibaba Cloud.

The table below shows how can we choose according to different scenarios:

| Source | Source Environment | Target     | Target Environment       | Requirement: Entire/Incremental/(Real-time/Cycle-synchronization) | Method      | Doc                                                          |
| ------ | ------------------ | ---------- | ------------------------ | ------------------------------------------------------------ | ----------- | ------------------------------------------------------------ |
| oracle | on-premises        | maxcompute | public cloud             | entire+incremental+real-time                                 | dts+mysql   | [orcl-op-maxc-pub-entire-incr-rt-dts](orcl-op-maxc-pub-entire-incr-rt-dts/README.md) |
| oracle | on-premises        | maxcompute | public cloud             | entire+incremental+realtime                                  | dts+datahub | orcl-op-maxc-pub-entire-incr-rt-datahub                      |
| oracle | on-premises        | mysql      | on-premise/private cloud | entire+incremental+cycle-synchronization                     | kettle      | orcl-op-maxc-op-entire-incr-cycl                             |

For example, the first article describe the situation of extracting data from oracle database from on-premise environment to maxcompute on public cloud, firstly we migrate the full data at one time, followed by real-time incremental data synchronization to MaxCompute.

