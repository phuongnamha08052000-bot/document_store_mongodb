# document_store_mongodb
Explored a document database workflow with MongoDB

Overview:
I explored a document database workflow by loading a curated companies JSON (public/company info) into MongoDB, then answering business questions with find/regex and aggregation pipelines (sums, grouping, sorting). Great contrast to the relational project above. 

Process:
Load & verify: Inserted a list of company JSON documents; validated counts/shape.
Targeted finds: Queried companies founded ≥ 1990 and sorted by employees (ascending).
Regional revenue splits: Aggregated total revenue for US-headquartered companies and selected European countries via $match + $group.
Text/regex search: Matched descriptions containing “second-largest … crude oil reserves” to identify Saudi Aramco and return its country.
Top-revenue query: Among companies founded < 1970, returned the one with the largest annual revenue.
Sector rollup: Computed total revenue and employees for an energy cohort using a regex-based $match.
Skills: MongoDB CRUD, regex filters, aggregation framework, schema-light analytics.
