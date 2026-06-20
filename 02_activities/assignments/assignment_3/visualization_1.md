# Visualization 1: Library Circulation by Cardholder Type (2022 vs 2023)

**Dataset:** Library Circulation by Cardholder Type, Toronto Public Library
**Source:** https://open.toronto.ca/dataset/library-circulation-by-cardholder-type/

---

**What software did you use to create your data visualization?**

I used Python, specifically the matplotlib library, to create a grouped bar chart.

**Who is your intended audience?**

The intended audience is Toronto Public Library administrators and city policymakers who are interested in understanding circulation trends across different age groups (Child, Teen, Adult) to inform program planning and resource allocation.

**What information or message are you trying to convey with your visualization?**

The visualization shows that Adult cardholders account for the overwhelming majority of total library circulation, far exceeding Child and Teen circulation combined. It also shows a slight year-over-year decline in circulation across all three cardholder types from 2022 to 2023.

**What aspects of design did you consider when making your visualization? How did you apply them? With what elements of your plots?**

I applied several design principles covered in this course:
- *Data-ink ratio* (Tufte, 2001): I removed the top and right chart borders (spines) to reduce unnecessary visual elements and keep focus on the data itself.
- *Clarity and precision*: I added exact data labels above each bar so viewers do not need to estimate values from the y-axis alone.
- *Comparison*: I used a grouped bar chart (rather than a single bar or pie chart) because it allows direct, accurate comparison of values across two dimensions (Year and Cardholder Type) using position and length, which research shows are the most accurately perceived visual encodings (Cleveland & McGill, 1984).

**How did you ensure that your data visualizations are reproducible? If the tool you used to make your data visualization is not reproducible, how will this impact your data visualization?**

The Python script is fully reproducible: it loads the raw CSV directly, performs all aggregation steps in code (rather than manually in a spreadsheet), and is run inside a dedicated virtual environment (`visualization-env`) with pinned package versions. Anyone with the same CSV file and environment can run the script and generate an identical chart.

**How did you ensure that your data visualization is accessible?**

I used a colorblind-friendly color palette (teal and tomato, which have sufficient contrast and are distinguishable from common forms of color vision deficiency), added a clear legend, used high color contrast against a white background, and included data labels so the information is not solely dependent on color perception or precise bar-height estimation.

**Who are the individuals and communities who might be impacted by your visualization?**

Library patrons of all ages, particularly families and youth who rely on library services, could be impacted if this data is used to make funding or program decisions. For example, lower Teen circulation might be interpreted as declining interest, which could affect investment in teen programming, even though other factors (e.g., digital reading habits not captured in this physical circulation dataset) may explain the trend.

**How did you choose which features of your chosen dataset to include or exclude from your visualization?**

The original dataset includes a `BranchCode` column with 114 individual branches. I excluded branch-level detail in this visualization and aggregated circulation citywide, because the goal was to convey an overall trend by cardholder type rather than branch-specific performance, which is the focus of Visualization 2.

**What 'underwater labour' contributed to your final data visualization product?**

Significant work went into data cleaning and exploration before visualization: inspecting the dataset for missing values, understanding the granularity of the data (per-branch, per-year), deciding on an appropriate aggregation method (summing across branches), and testing several chart types (e.g., stacked bar, line chart) before settling on a grouped bar chart as the clearest way to compare both year and cardholder type simultaneously.

---

## References

Cleveland, W. S., & McGill, R. (1984). Graphical perception: Theory, experimentation, and application to the development of graphical methods. *Journal of the American Statistical Association*, 79(387), 531–554.

Tufte, E. R. (2001). *The visual display of quantitative information* (2nd ed.). Graphics Press.