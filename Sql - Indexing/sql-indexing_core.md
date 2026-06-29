
[Clustered vs Non-Clustered](https://app.notion.com/p/Clustered-Non-Clustered-38ea04c1c6bd8075ba1ceb4583d9a7cd?source=copy_link) -->


# SQL Indexing Diagram

```mermaid
flowchart TD
    A[SQL Indexing] --> B[Index Types]
    B --> B1[B-tree / B+Tree]
    B --> B2[Hash Index]
    B --> B3[Bitmap Index]
    B --> B4[GIN / GiST / BRIN - Postgres]
    B --> B5[Covering]
    B --> B6[Unique]
    B --> B7[Clustered vs Non-Clustered]

    A --> C[Operations Supported]
    C --> C1[Equality Search]
    C --> C2[Range Search]
    C --> C3[Sorting / ORDER BY]

    A --> D[Factors to Consider]
    D --> D1[Cardinality - Distinct Values]
    D --> D2[Selectivity - Filtering Power]
    D --> D3[Query Patterns - WHERE, JOIN, ORDER BY]
    D --> D4[Composite Indexes]
