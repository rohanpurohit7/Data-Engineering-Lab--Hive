# Project Context

## Problem

This project uses Apache Hive to analyze MovieLens-style rating data with SQL over Hadoop storage. The workflow stages ratings, validates table structure, enriches event time into weekday features, and aggregates activity by time dimension.

## Data Engineering Flow

Ratings file -> Hadoop storage -> Hive staging table -> schema validation -> timestamp enrichment -> analytical table -> SQL aggregation -> result validation.

## Domain Interpretation

The lab demonstrates how raw event records become analytics-ready dimensions. Converting Unix timestamps into weekday categories supports behavioral analysis such as identifying when rating activity is highest.

## Data Quality Questions

- Does the delimiter match the source format?
- Are user, movie, rating, and timestamp fields typed correctly?
- Are timestamps interpreted in the intended timezone?
- Are row counts preserved after transformation?
- Are null or malformed rows isolated?

## Validation

Validate source counts, table schema, sample rows, transformation output, grouped counts, and repeatability.

## Use Cases

SQL-on-Hadoop analytics, warehouse staging, behavioral analytics, feature engineering, and modernization to Spark SQL, Trino, Athena, Databricks SQL, or lakehouse architectures.

## Public-Artifact Standard

Use public datasets and generic environment references. Remove personal identifiers, account identifiers, private hostnames, internal paths, private network details, credentials, tokens, and organization-specific information before publication.
