#testing 

= EC

**Basic Idea:** The domain of input and output values is partitioned into Equivalence Classes. All values within a single EC are assumed to lead to the same behavior. A single arbitrary value is chosen from each class as a representative sample.

**Procedure for Defining ECs:**

- **[[Domain Constraint]] (e.g., range 1 to 100):** Create one valid EC (1 <= x <= 100) and two invalid ECs (x < 1 and x > 100).
- **[[Min/Max Number Constraint]]:** Create one valid EC and two invalid ECs.
- **[[Set of Values]] (treated differently):** Create one valid EC for every specified value, plus one overall invalid EC for everything else (e.g., Badminton vs. Football).
- **[[Situation Fulfillment Constraint]]:** Create one valid EC and one invalid EC.

**[[Test Case]] Minimization and [[Failure Masking]]:**

- The minimal criteria require at least one representative of each EC to be included in at least one test case.
- Combining representatives of invalid ECs should be avoided because it can lead to **potential [[failure masking]]**.
- Test End Criteria: **[[EC-Coverage]]** is calculated as (No. of tested EC / Total no. of EC) * 100%.
- _Advice:_ For selecting powerful test data, combine EC with failure-oriented methods like boundary value analysis.

**[[Combinatorial Interaction Testing]] (CIT):** CIT aims to minimize the test cases while covering combinations of ECs.