# This project processes a raw dataset of Olympic athletes (bios.csv) to create a cleaned version. The goal is to separate merged information into distinct columns for easier filtering and calculation.

# Key Data Transformations
### The following cleaning steps were performed:

Name Formatting: Removed special characters (•) from athlete names.

Physical Metrics: Split the Measurements column into separate numeric height_cm and weight_kg columns.

Geographic Extraction: Parsed the Born text to extract specific born_city, born_region, and born_country codes.

Date Parsing: Extracted birth and death dates into standardized formats for chronological analysis.

Column Reduction: Removed unnecessary metadata to focus on core biographical facts.

# Tools Used
Python: Primary programming language.

Pandas: For data manipulation and CSV export.

Regex (Regular Expressions): Used to identify and extract patterns within text strings.

# Final Dataset Structure
The cleaned output includes:

athlete_id: Unique identifier for each athlete.

name: Cleaned full name.

born_date / died_date: Standardized dates.

born_city / born_region / born_country: Detailed birth location.

height_cm / weight_kg: Numeric physical attributes.
