# Cafe Sales Data Cleaning Project

This project demonstrates practical data cleaning and standardization skills using Excel on a real-world messy dataset.

## Key Skills Demonstrated
- Handling missing values
- Data standardization
- Data reconstruction
- Data preparation for analysis


OVERVIEW:
   This project focuses on cleaning and standardizing a raw cafe sales dataset to improve data quality and prepare it for further analysis.

2. IDENTIFIED ISSUES IN RAW DATASET:
   Several data quality issues were identified in the original dataset:

	Inconsistent Column Formatting

		-Column widths were not properly adjusted, making the dataset difficult to read.

	Unstandardized Column Names

		-Column names were inconsistent in formatting (e.g., spacing, capitalization).

	Missing Values

		-Several columns contained missing values, particularly:

		   >quantity

		   >price_per_unit

		   >total_spent

	Unsorted Data

		-Transaction records were not ordered, reducing readability and usability.

3. Data Cleaning & Transformation Steps
   The following steps were performed to address the issues:

	Improving Readability

		-Adjusted column widths to fit content for better visibility and usability.

	Standardizing Column Names

		-Applied consistent naming conventions:

		   >Removed unnecessary spaces using TRIM()

		   >Standardized capitalization using PROPER()

		   >Replaced spaces with underscores (_) for better compatibility in analysis tools

	Handling Missing Values

		-Reconstructed missing values where possible:
			>total_spent = quantity × price_per_unit
			>quantity = total_spent / price_per_unit
			>price_per_unit = total_spent / quantity
	This approach was used to preserve as much data as possible without removing rows.
	Some values remain missing due to insufficient data.

Note:
Future improvement: missing price_per_unit values can be inferred using lookup methods (e.g., Excel XLOOKUP or VLOOKUP) based on similar item names


	Sorting Data

		-Sorted dataset by transaction_date to improve structure and analytical readiness

4. Results

	After cleaning:

		-Dataset is more structured and readable

		-Column naming is consistent and analysis-friendly

		-Missing values have been partially resolved

		-Data is now better organized for further analysis using tools such as Excel, SQL, or Python

5. Future Improvements
   Implement lookup techniques (e.g., XLOOKUP) to further reduce missing values
   Perform validation checks for data consistency
   Extend analysis to extract business insights (e.g., sales trends, top-selling items)
