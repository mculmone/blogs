# Filtering log data with New Relic Logs

## Overview

### What is a drop filter

After log event data has been shipped to New Relic, it can either be stored in our database (NRDB  ) or dropped (discarded). New Relic Logs can drop both log events and event attributes via drop filter rules. You can manage drop filter rules using New Relic Logs or NerdGraph.

### Why are they useful

Drop filter rules help you accomplish some very important goals:

You lower costs by storing only logs relevant to your account.
You protect privacy and security by removing personal identifiable information (PII).
You reduce noise by removing irrelevant events and attributes.

### How they work

A drop filter rule matches data based on a query. When triggered, the drop filter rule removes the matching data from the ingestion pipeline before it is written to in NRDB. Since the data does not reach the backend, it cannot be queried: the data is gone and cannot be restored.A

## Examples

### Example 1 -

### Example 2 -

## Resources and Support

The New Relic documentation for logs [https://docs.newrelic.com/docs/logs/](https://docs.newrelic.com/docs/logs/) contains a section on using [drop filters](https://docs.newrelic.com/docs/logs/new-relic-logs/ui-data/drop-data-drop-filter-rules) and how they work.
