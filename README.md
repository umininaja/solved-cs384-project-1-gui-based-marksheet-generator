Download Link: https://assignmentchef.com/product/solved-cs384-project-1-gui-based-marksheet-generator
<br>
When the quiz is conducted on Google Form, Google does not provide an option for computing -ve marking. It gives 0 marks for wrong answer. It just gives a csv file as output for post processing. Your task is to make a standalone GUI/web based interface that will have such an option. <strong>Web based is a preferred method in this project.</strong>

<strong>Input: </strong>You are given a <strong>.csv </strong>file that contains marks for each roll number and the individual options marked by each students(see sample inputresponses.csv). The following first seven columns are fixed:

<strong>Timestamp: </strong>At what time student submitted their question paper.

<strong>Email address: </strong>Email address to which student login.

<strong>Score: </strong>Total calculated score.

<strong>Name: </strong>Name of the student.

<strong>IITP webmail: </strong>IITP webmail address. <strong>Phone number: </strong>Phone number of the student <strong>Roll Number: </strong>Roll number of the student.

<strong>Outputs</strong>

<ol>

 <li>Your aim is to make a GUI as shown in Figure 1. Here the first button is to upload a master roll.csv file. It contains the names and roll number of all the students of the class. (see sample inputmaster roll.csv)</li>

 <li>Next is the response sheet csv obtained from google (see sample inputresponses.csv). You need to check that a row with roll number ANSWER should be present in this file. If not, pop and error saying that, “no roll number with ANSWER is present, Cannot Process!”. A user with select the browse button and select these two files.</li>

 <li>Next, the user will be asked to enter the number of +ve and -ve marks. In this case as shown in Fig. 1, +5 is for correct answer and -1 is for wrong ans. 0 is a valid input for -ve cases. Assume that correct numbers r being entered here, decimal being allowed. So +4.5, and -1.25 is a valid input.</li>

 <li>All the output files should be in the folder named “marksheets”</li>

 <li><strong>Generate Roll Number wise marksheet</strong>. Here you need to generate a marksheet for every roll number present in the master roll. If a roll number is present in the master file but not in the response.csv that means that student was absent, so a blank marksheet file needs to be generated having all answers as blank. This option also will generate a marksheet of individual roll number and save as ”.xlsx”. A sample ”1401ME06.xlsx” is provided for your reference. Its self explainable. The number of right answers, number of wrong answers, not attempted questions and the marks associated with right, wrong answers are displayed after being calculated automatically. Please maintain the font colors. Master Key answers are in Blue, Student’s correct answer is in Green and wrong answer are in red. Refer ”1401ME06.xlsx” for color scheme. The file should also have the IITP logo.</li>

</ol>

1

Figure 1: GUI Options. On the right you are given the option for +ve and -ve marks. In this example, it depicts that 5 mk are for correct answer, and -1 is for wrong. This input should be dynamic, so calculations should be based on the input provided. 0 is also a valid input for -ve case.

<ol start="6">

 <li>A generate concise marksheet option is given that contains all the marked options as well as marks before and after -ve computation. (see sample outputmarksheetconcise marksheet.csv)</li>

 <li>So, for a class of k roll numbers, there will be k output xlsx files, and 1 summary file (concise marksheet.csv) that contains the concise info for marks before and after negative.</li>

 <li>Make sure all the roll number based are saved with uppercase roll numbers. So if the person has entered 1701cs45 in the response.csv, it should be always saved as 1701CS45.xlsx</li>

 <li>Add a button namely <strong>Send Email </strong>and when you click on send email button, it will send a marksheet to you email address with the marksheet of that roll number. Email should be done on both emails of response sheet.</li>

 <li>For frontend, any web technologies can be used. But backend csv processing needs to be Python Sample Input and Output are provided</li>

</ol>


