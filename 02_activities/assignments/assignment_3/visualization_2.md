# Visualization 2: Top 15 Toronto Public Library Branches by Circulation (2023)

**Dataset:** Library Circulation by Cardholder Type, Toronto Public Library
**Source:** https://open.toronto.ca/dataset/library-circulation-by-cardholder-type/

---

**What software did you use to create your data visualization?**

I used Microsoft Excel to create a horizontal bar chart.

**Who is your intended audience?**

The intended audience is Toronto Public Library branch managers and resource planning staff who need a quick, branch-level view of where circulation demand is highest, to inform staffing and collection allocation decisions.

**What information or message are you trying to convey with your visualization?**

The visualization highlights that one branch (VIR) accounts for a disproportionately large share of total circulation compared to all other top branches combined — over 12.3 million items in 2023, nearly 20 times higher than the second-highest branch (CL, at 616,108). This signals that VIR likely functions differently from typical neighbourhood branches (e.g., as a central/reference library) and may warrant separate consideration in resource planning.

**What aspects of design did you consider when making your visualization? How did you apply them? With what elements of your plots?**

I used a horizontal bar chart rather than a vertical one because branch codes are categorical labels of varying length, and horizontal bars make these labels easier to read without rotation (Few, 2012). I sorted bars in ascending order so the largest value (VIR) draws the eye at the top, following a natural reading pattern. I also added precise data labels directly on each bar, since the extreme difference between VIR and other branches would otherwise be difficult to judge accurately on a shared axis scale.

**How did you ensure that your data visualizations are reproducible? If the tool you used to make your data visualization is not reproducible, how will this impact your data visualization?**

This visualization is less reproducible than Visualization 1, since Excel chart formatting (colors, label positions, chart type selections) was done manually through the GUI rather than through code. However, the underlying data subset (`top15_branches_2023.csv`) was generated reproducibly using Python (see appendix code), so while the exact visual styling in Excel would need to be manually recreated, the data itself can be regenerated identically by anyone re-running the Python script. This is a limitation of GUI-based tools: a future user re-running the workflow would need to repeat the manual Excel formatting steps to obtain an identical-looking chart.

**How did you ensure that your data visualization is accessible?**

I used a single consistent color (teal, matching Visualization 1) with high contrast against a white background, large readable font sizes for branch labels, and included exact numeric labels so the information does not rely solely on visually estimating bar length, which assists viewers with visual impairments.

**Who are the individuals and communities who might be impacted by your visualization?**

Library patrons in neighbourhoods served by lower-circulation branches could be impacted if this visualization is used to justify reduced resources for those branches. It is important to note that circulation volume alone does not capture community need; smaller branches in underserved neighbourhoods may have lower circulation due to fewer registered cardholders, not because the library service is less valued there.

**How did you choose which features of your chosen dataset to include or exclude from your visualization?**

I excluded the `CardholderType` breakdown used in Visualization 1 and instead aggregated total circulation per `BranchCode` for the most recent year (2023) only, to focus this visualization on geographic/branch-level patterns rather than demographic patterns, ensuring the two visualizations are clearly distinct in purpose.

**What 'underwater labour' contributed to your final data visualization product?**

I wrote a Python script to aggregate and export the top 15 branches by circulation, which required deciding on a threshold (top 15, rather than all 114 branches) to keep the chart readable. I then manually experimented with chart type (vertical vs. horizontal bar), sort order, and label placement in Excel to find the clearest layout, and cross-referenced the branch code list to understand which branch "VIR" represents.

---

## References

Few, S. (2012). *Show me the numbers: Designing tables and graphs to enlighten* (2nd ed.). Analytics Press.