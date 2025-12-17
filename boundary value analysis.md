#testing 

= BVA

**Basic Idea:** Failures often occur at boundaries (where a constraint just holds or just fails to hold), leading to "off by one" errors. BVA tests these specific boundary values to increase the likelihood of finding failures.

![[Screenshot 2025-12-04 at 04.32.17.png]]

**Procedure:**

- BVA is best used in combination with [[equivalence class|Equivalence Classes]].
- Test the lowest (`l`) and greatest (`g`) value of an EC.
- Extend the values to include inputs right and left of the boundary (e.g., valid and invalid values near the threshold).
- Always test two values for every boundary: the boundary value itself, and the value immediately before/after the boundary.
- For set-based domains (e.g., data structures), test the smallest and biggest valid quantities, and the smallest and biggest invalid quantities.

**Assessment:**

- **Pro:** Boundaries often contain more failures than values within the class.
- **Contra:** Defining all boundary values can be very complex, and selecting test data requires creativity without a clear "recipe".
- Test End Criteria: **[[BV-Coverage]]** is calculated as (No. of tested BV / Total no. of BV) * 100%.