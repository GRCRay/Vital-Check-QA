| Test ID | Metric | Input Value | Category | Expected Result |
| :---| :---| :---| :---| :---|
| BVA-01 | Blood Pressure | 120/80 | Valid | System accepts and saves record |
| BVA-02 | Blood Pressure | 0/0 | Min Boundary | "System rejects; Error: ""Invalid reading" |
| BVA-03 | Blood Pressure | 300/200 | Max Boundary | System saves; Triggers High Alert |
| BVA-04 | Blood Sugar,20 | Low Boundary | System saves; Triggers Hypoglycemic Alert |
| BVA-05 | Blood Sugar | abc | Invalid | "System rejects; Error: ""Numeric only" |
