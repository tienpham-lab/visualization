# Data Visualization

## Assignment 2: Good and Bad Data Visualization

### Requirements:

- Data visualizations are important tools for communication and convincing; we need to be able to evaluate the ways that data are presented in visual form to be critical consumers of information 
- To test your evaluation skills, locate two public data visualizations online, one good and one bad  
    - You can find data visualizations at https://public.tableau.com/app/discover or https://datavizproject.com/, or anywhere else you like! 
- For each visualization (good and bad):  
    - Explain (with reference to material covered up to date, along with readings and other scholarly sources, as needed) why you classified that visualization the way you did.
      ```
      
      The Choropleth Map (https://datavizproject.com/data-type/choropleth-map-2/) is a good data visualization for three key reasons.
      
      First, it excels in substantive quality by effectively communicating geographic distribution of data. By shading regions in proportion to a statistical variable such as population density or income, viewers can immediately identify spatial patterns and regional disparities (Domo, 2026).
      
      Second, it demonstrates strong perceptual quality. A sequential color scale aligns with human perception - darker colors naturally signal higher values, reducing cognitive load (Felt, 2025). This makes the map intuitive without requiring technical knowledge.
      
      Third, its aesthetic quality supports rather than distracts from communication. A clean layout with a clear legend avoids unnecessary visual clutter, keeping focus on the data (U.S. Data Design Standards, n.d.).

      The 3D Bar Chart (https://datavizproject.com/data-type/3d-bar-chart/) is a poor data visualization for three key reasons.
      
      First, it fails in perceptual quality due to perspective distortion. Bars at the back appear shorter than bars at the front even when representing equal values, causing viewers to misread the data (Purohit, 2021). Research confirms that humans judge position along a common scale far more accurately than angles or distorted areas (Cleveland & McGill, as cited in arxiv, 2019).
      
      Second, it lacks substantive quality. The third dimension adds no additional data — it is purely decorative. This violates the principle of maximizing the data-to-ink ratio, where all visual elements should serve the data (Kilin, 2024).
      
      Third, occlusion undermines aesthetic and functional quality. Bars in front can block bars behind entirely, making some data points invisible and comparisons impossible (Domo, 2024).  
      
      **References**
      Cleveland, W. S., & McGill, R. (1984). Graphical perception: Theory, experimentation, and application to the development of graphical methods. *Journal of the American Statistical Association*, 79(387), 531–554. As cited in Morais, L., et al. (2019). *Let's gamble: Uncovering the impact of visualization on risk perception and decision-making*. arXiv. https://arxiv.org/pdf/1910.09725
      Domo. (2026a). *3D charts: When to use them and when to avoid them*. https://www.domo.com/learn/charts/3d-charts
      Domo. (2026b). *Choropleth maps explained: Examples, uses, and tips*. https://www.domo.com/learn/charts/choropleth-maps
      Felt. (2025). *Choropleth maps: Color-coding patterns without misleading your audience*. https://felt.com/blog/choropleth-maps
      Kilin, I. (2024). *Bad data visualization: How to notice and fix it (27 examples)*. Datylon. https://www.datylon.com/blog/bad-data-visualization-examples
      Purohit, P. (2021, December 15). *Data visualization: Why 3D charts are a terrible idea*. Medium. https://medium.com/@purohitpraveen/data-vizualization-why-3d-charts-terrible-idea-32657fbb928e      
      U.S. Data Design Standards. (n.d.). *Choropleth map*. https://xdgov.github.io/data-design-standards/visualizations/choropleth-map

      ```
    - How could this data visualization have been improved?  
      ```
      **For the Choropleth Map**

      First, color palette choices could be more accessible. Red-green contrasts are difficult for colorblind viewers; using colorblind-friendly palettes such as viridis would improve equity (Felt, 2025).
      
      Second, adding interactive tooltips showing exact values when hovering over regions would improve precision, as choropleth maps tend to communicate general patterns rather than specific numbers.
      
      **For the 3D Bar Chart**
      
      First, replacing the 3D chart with a standard 2D grouped bar chart would immediately improve readability, allowing accurate comparison against a flat baseline.
      
      Second, adding data labels to each bar would compensate for the difficulty of reading exact values, directly improving both substantive and perceptual quality.

      ```
- Word count should not exceed (as a maximum) 500 words for each visualization (i.e. 
300 words for your good example and 500 for your bad example)

### Why am I doing this assignment?:

- This assignment ensures active participation in the course, and assesses the learning outcomes
* Apply general design principles to create accessible and equitable data visualizations
* Use data visualization to tell a story

### Rubric:

| Component               | Scoring   | Requirement                                                 |
|-------------------------|-----------|-------------------------------------------------------------|
| Data viz classification and justification | Complete/Incomplete | - Data viz are clearly classified as good or bad<br />- At least three reasons for each classification are provided<br />- Reasoning is supported by course content or scholarly sources |
| Suggested improvements  | Complete/Incomplete | - At least two suggestions for improvement<br />- Suggestions are supported by course content or scholarly sources |

## Submission Information

🚨 **Please review our [Assignment Submission Guide](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md)** 🚨 for detailed instructions on how to format, branch, and submit your work. Following these guidelines is crucial for your submissions to be evaluated correctly.

### Submission Parameters:
* Submission Due Date: `23:59 -  2026-06-09`
* The branch name for your repo should be: `assignment-2`
* What to submit for this assignment:
    * This markdown file (assignment_2.md) should be populated and should be the only change in your pull request.
* What the pull request link should look like for this assignment: `https://github.com/<your_github_username>/visualization/pull/<pr_id>`
    * Open a private window in your browser. Copy and paste the link to your pull request into the address bar. Make sure you can see your pull request properly. This helps the technical facilitator and learning support staff review your submission easily.

Checklist:
- [ ] Create a branch called `assignment-2`.
- [ ] Ensure that the repository is public.
- [ ] Review [the PR description guidelines](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md#guidelines-for-pull-request-descriptions) and adhere to them.
- [ ] Verify that the link is accessible in a private browser window.

If you encounter any difficulties or have questions, please don't hesitate to reach out to our team via our Slack. Our Technical Facilitators and Learning Support staff are here to help you navigate any challenges.
