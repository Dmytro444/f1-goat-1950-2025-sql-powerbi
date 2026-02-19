# F1 GOAT 1950-2025
Analytical project evaluating historical performance of drivers competing in Formula 1 (1950-2025) using standardized scoring systems and cross-era normalization techniques.

## Objective
Comparing drivers across different eras is statistically challenging due to:
- changing points scoring systems;
- varying number of races per season;
- mechanical reliability differences;
- team performance gaps.

This project aims to normalize historical data and evaluate drivers using a consistent analytical framework.

## Dataset overview
- 27291 race-result records;
- 1149 Grand Prix events;
- ~800 drivers;
- 76 seasons;
- 17 data model tables.

## Analytical framework
Drivers were evaluated using four key dimensions:
1. Championship performance under:
    - historical points systems,
    - full-season actual race points,
    - modern points scoring system,
    - custom top-15 scoring system.
2. Career titles under each scoring system.
3. Average finishing position (minimum 20 races across 3 seasons)
4. Head-to-head performance vs teammates (minimum 10 comparable races across 3 seasons).

Bonus analysis: age vs performance trends.

## Tech stack
- SQL (extraction, joins, aggregations);
- Excel + VBA (data enrichment, handling exceptions, determining thresholds);
- Power Query (ETL, data cleaning, advanced grouping and transformation);
- Power BI (data model, DAX measures, interactive dashboards).

## Key insights
- Normalizing scoring systems significantly changes historical title distribution.
- Head-to-head teammate dominance often provides a stronger performance indicator than raw championship count.
- Results from the early decades were significantly distorted by machinery's reliability.
- Average champions' age tends to decrease in recent decades.

## Data source
[Open Source Formula 1 Database](https://github.com/f1db/f1db) (v2025.24.2)

## Additional documentation
Detailed step-by-step explanation of the data processing and modeling pipeline is available in the [Technical implementation](https://github.com/Dmytro444/f1-goat-1950-2025/blob/48b1815e5881091b00f8e89eaf94ccd0c9f0c719/Technical%20implementation.md) file.
