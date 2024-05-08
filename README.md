# Validation_courses_extension
validations of the extension course templates with parameters requested by the Colombian Ministry of Education

# Project description
My role was as the programmer, and my responsibility was the design and entire development of this project.

I developed a Python code aimed at enhancing the efficiency and accuracy of data management for government forms (ESNIES) related to extension courses. This initiative resulted in a significant reduction in review time, thereby streamlining the management process. Despite dealing with a high volume of information, the project was executed meticulously, demonstrating adept organizational skills and a structured architecture. Moreover, to facilitate understanding and execution, comprehensive tutorials were created, showcasing strong communication abilities.
The implementation of a try-catch structure within the code ensured resilience against potential errors, preventing interruptions and maintaining the smooth operation of the program.

Here are additional details:

•  Performing this task manually could take 5 days, and a human could make various errors. Meanwhile, running my code takes only about 7 or 8 minutes.

•  There were 7 different government forms (each form is an Excel file), and each Excel file has several sheets. Each sheet has several columns, and each column has different validations of type numeric/alphanumeric, data length, valid values, and other even more customized validations, such as email validation, negative values, whether end dates are later than start dates, some values depending on the existence of a previous field, among others.

•  To achieve this, I used numpy and pandas libraries, among others, such as drive, pathlib, email_validator, datetime, etc. I also used structures for handling errors, such as try and except.

•  First, I generated some general functions to be used later in more personalized functions.

•  The architecture of the code is such that I created a Jupyter notebook and generated a section for each template. In total, there were 7 sections.

Within each section, I have the same structure: 4 functions per section:

1.  One function takes the path where all those Excel files to be evaluated are located and iterates through them for validation.

2. Another function takes one file and validates it. First, it generates empty variables, and then some customized functions evaluate and validate all the sheets and their columns, returning the variables with the results.

3. This part is not a single function, but the compendium of all custom functions per column. This is where the customized functions are defined, one function per column, and inside is where the general functions are applied depending on the validation defined by the government.

4. Finally, I generate an Excel file with the results. The first sheet is a general report with the fields found, the ones not found, the date and time when this validation was made, and some other general data such as the faculty and data related to the faculty and the courses. The rest of the sheets of this report have a 'mirror' of the original form but indicate which data doesn't comply with the requirements and why. For example, cell A3 is required to have a length of 1 character, but its current value length is 2.

Another point to showcase in this project is the explanation of how to use it correctly, with many details, screenshots, and examples of good and wrong cases that demonstrate the ability to communicate with others.
I designed the entire code in a notebook separate from the execution notebook to avoid incorrect editions and to enhance the visual experience.

I recognize that the code could be improved significantly. This design was chosen at the request of my boss, as the code was to be manipulated by individuals with varying levels of expertise in Python. That's why I didn't use classes or object-oriented programming (OOP) or other more complex structures.

# What was the outcome of the project?
The implementation of the Python code not only expedited the review process but also ensured the maintenance of data integrity and quality. By adhering to a simple syntax without utilizing classes or objects logic, the solution was accessible to individuals with varying levels of Python proficiency, as per the directive from senior management. Ultimately, this project underscored the ability to deliver practical solutions that align with organizational goals while catering to user requirements and constraints.
