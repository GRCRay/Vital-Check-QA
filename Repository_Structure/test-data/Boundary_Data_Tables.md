| Test ID | Metric | Input Value | Category | Expected Result | Actual Results | Status |
| :---| :---| :---| :---| :---| :---| :---|
| BVA-01 | Blood Pressure | 120/80 | Valid | System accepts and saves record | System accepts and saves record | PASS |
| BVA-02 | Blood Pressure | 0/0 | Min Boundary | "System rejects; Error:" "Invalid reading" | System accepts and saves record | FAIL |
| BVA-03 | Blood Pressure | 300/200 | Max Boundary | System saves; Triggers High Alert | "System rejects; Error:" "Invalid reading" | FAIL |
| BVA-04 | Blood Sugar | 20 | Low Boundary | System saves; Triggers Hypoglycemic Alert | System accepts and saves record | FAIL |
| BVA-05 | Blood Sugar | abc | Invalid | "System rejects; Error:" "Numeric only" | System did accept "abc" input | PASS |
