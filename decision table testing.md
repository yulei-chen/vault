#testing 

= DT

**Applicability:** DT is applicable for complex rules and system requirements involving logical conditions, particularly in business processes.

**Structure and Components:**

- **Conditions:** Possible states of objects (can be True 'T', False 'F', or Insignificant '-').
- **Rules (Columns):** Combinations of condition values.
- **Actions:** Activities executed based on the rules (marked with 'X' for execute).
- **Action Pointer:** Allocates conditions with actions.

**Analysis and Test Cases:**

- The decision table is **complete** if  combinations are defined for  conditions.
- The DT is **redundancy free** if specific conditions lead to different actions.
- The DT is **consistent** if the same conditions lead to the same actions.
- **Test Cases:** Every column (rule) in the decision table corresponds to one test case.

**Assessment:**

- **Pro:** Systematically formulates logical coherences and derives condition combinations that might not be executed otherwise. DTs are easily checked for redundancy, consistency, and completeness.
- **Contra:** DTs become confusing if there are too many conditions.