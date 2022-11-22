[![REUSE status](https://api.reuse.software/badge/github.com/SAP-samples/teched2022-DT263)](https://api.reuse.software/info/github.com/SAP-samples/teched2022-DT263)

# DT263 - Experience SAP S/4HANA Localization as a Self-Service 

## Description

This repository contains the material for the Session ID - DT 263 - Experience SAP S/4HANA Localization as a Self-Service 

## Overview

This session introduces attendees to how true global compliance can be achieved seamlessly by leveraging the extensibility capabilities of SAP Document and Reporting Compliance - Statutory Reporting 

## Requirements

The participants of this hand-on should have sufficient knowledge on the following topics: 
- Basic knowledge of SAP S/4HANA 
- Basic knowledge of Indirect Tax like VAT, GST etc. 
- Basic understanding of xml, xsd : Nice to have in case they require legal reports in this format 
- S/4 Finance Data Model basic understanding: BKPF, BSET etc. 

## Exercises

In these exercises, we will learn how to fulfill statutory reporting requirements for custom local versions by easily extending the standard generic reuse objects provided by SAP Document and Reporting Compliance - Statutory Reporting   We have the following requirements:  

1. We have to create a VAT statutory report for the country Latvia which is a custom local version
2. The legal authorities have mandated the reporting of VAT line items in the statutory report
3. These VAT line items have to be reported in a file with the format TXT
4. Each VAT line item must be delimited by ';'

- [Getting Started](exercises/ex0/)
- [Exercise 1 - Creating an extension of generic report definition](exercises/ex1/)
- [Exercise 2 - Creating a custom report category](exercises/ex2/)
- [Exercise 3 - Using "Run Statutory Reports" app to generate a report](exercises/ex3/)


## How to obtain support

Support for the content in this repository is available during the actual time of the online session for which this content has been designed. Otherwise, you may request support via the [Issues](../../issues) tab.

## License
Copyright (c) 2022 SAP SE or an SAP affiliate company. All rights reserved. This project is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE](LICENSES/Apache-2.0.txt) file.
