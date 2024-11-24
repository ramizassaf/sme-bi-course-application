# Virtual Machine (VM) Exercises

## :information_source: Read this before getting started
- The two exercises should not replicate the exact actions shown in your screencast. The goal of exercises is for learners to apply what was learned in the screencasts to new problems or situations. This is best pedagogical practice for retaining and building skills. For example, this can be done by using another dataset between screencasts and exercises or focusing on a different portion of the dataset.
- Power BI / Tableau specific: We can only run free versions of BI software in our virtual machine exercises. In the case of Power BI, make sure the exercises can run on [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/) without any additional paid products. 
- Unsure what the scope of an exercise should be? Here's an [example](https://campus.datacamp.com/courses/introduction-to-power-bi/getting-started-with-power-bi?ex=14) from Introduction to Power BI. The first chapter of most DataCamp courses are free, so take a look at our [BI courses](https://learn.datacamp.com/courses?technologies=Tableau&technologies=Power%20BI) to get a feel for how we assess and guide learners.

## 1st VM Exercise

#### Dataset

- [ ] data_validation_ex2.xlsx

#### Files

- [ ] **Initial**: Add file to the `exercises/`  folder with the name `data_validation_ex2.xlsx` 
- [ ] **Solution**: Add file to the `exercises/`  folder with the name `data_validation_sol2.xlsx`

#### Learning Objective

Learners will be able to create complex data validation rules in Excel using formulas to restrict data entry based on multiple criteria.

#### Context

You are tasked with maintaining the integrity of a student enrollment spreadsheet for a training program. To ensure that only qualified students can enroll, you need to set up data validation that checks both the age and the enrollment status of the students.

#### Steps to be executed by the student (max 6)

- Open the Initial File: Download and open the provided initial Excel file named data_validation_ex2.xlsx.
- Select the Age Column: Click on the column that contains the students' ages (e.g., Column C).
- Apply Data Validation for Age:
    Go to the Data tab in the ribbon.
    Click on Data Validation.
- In the Data Validation dialog, select Custom from the "Allow" dropdown.
- Enter the proper formula [Hint: =AND(C2>=??, C2<= ??)] to ensure that students are between 18 and 30 years old.
- Select the Enrollment Status Column: Click on the column that indicates the enrollment status (e.g., Column D).
- Apply Data Validation for Enrollment Status:
- Repeat the data validation steps, but this time use the formula [=D2="??"] to restrict entries to only those who are currently enrolled.
- Add an Input Message: For both columns, add input messages to guide users. For the Age column: Title: "Age Input", Message: "Please enter an age between 18 and 30." For the Enrollment Status column: Title: "Enrollment Status", Message: "Please enter 'Enrolled' to register."
- Test the Validation: Try entering various ages and enrollment statuses to ensure that the validation works correctly. Test valid and invalid entries.
- Save Your Work: Save the file as Student_Enrollment_Validated.xlsx.

#### Exercise question:
What happens when you try to enter an age below 18 or above 30, or if you enter a status other than "Enrolled"? Provide examples of both valid and invalid entries for each column.

#### End goal:

You can use valication circles to see where invalid enrollment was made, click on the data validation icon group, second option.

## 2nd VM Exercise

#### Dataset

- [ ] data_validation_ex.xlsx

#### Files

- [ ] **Initial**: data_validation_ex.xlsx.
- [ ] **Solution**: data_validation_sol.xlsx

#### Learning Objective

Learners will be able to apply data validation techniques in Excel to ensure that inventory quantities are within acceptable limits.

#### Context

As a warehouse manager, you need to ensure that the quantities of items in your inventory database are valid. This exercise will help you set up data validation rules to prevent incorrect entries, such as negative quantities or critical items (items starting with E) being below 200 units on hand, which could lead to inventory errors.

#### Steps to be executed by the student (max 6)

- Open the Initial File: Download and open the provided Excel file named data_validation_ex.xlsx.
- Select the Quantity_on_hand Column: Click on the column that contains the quantities (e.g., Column C).
- Apply Data Validation:
    Go to the Data tab in the ribbon.
    Click on Data Validation.
- In the Data Validation dialog, select custom from the "Allow" dropdown.
- Set the proper rule, not less than 0, also less than 200 if the SKU starts with "E"
- Add an Input Message: In the same dialog, switch to the Input Message tab and check "Show input message when cell is selected". Enter a title and message to guide the user, e.g., Title: "Quantity Input", Message: "Please enter a quantity of 0 or more."
Test the Validation: Try entering various values in the Quantity_on_hand column to ensure that the validation works as expected. Enter a negative number and a valid number to see the different responses.
Save Your Work: Save the file as data_validation_ex_validated.xlsx.
#### Exercise question:
What error message appears when you try to enter a negative quantity? Provide an example of both a valid and an invalid entry.

#### End goal:

A table with invalid entried circled in red

