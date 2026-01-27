# Student Performance & Placement Analysis

<img width="1839" height="671" alt="image" src="https://github.com/user-attachments/assets/6fe1fec4-5458-42bc-89be-fe6b67f8f389" />


## 📌 Project Overview
Brief description of the project:
- The Objective of this analysis is to understand different distribution of students skills and achievements and How to make them better.
- Which Cretaria's matter for Student placements?
- This Dataset include numerous student details regarding their technical & academic skills, which makes it right for this analysis.

---

## 📂 Dataset Overview
- This dataset was gathered from Kaggle by <a href="https://www.kaggle.com/datasets/suvidyasonawane/student-academic-placement-performance-dataset">Student Academic Placement Performance Dataset</a>.
- There are data of 5000 students with 18 different features including student_id
- Brief description of key columns  
  - gender : Student's Gender
  - ssc_percentage : 10<sup>th</sup> Percentage
  - hsc_percentage : 12<sup>th</sup> Percentage
  - degree_percentage : Degree Percentage
  - cgpa : Degree CGPA
  - entrance_exam_score : College Entrance Exam Score
  - technical_skill_score : Technical Skill Score
  - soft_skill_score : Soft Skill Score
  - internship_count : No. of Intership Done
  - live_projects : No. of Projects Completed
  - work_experience_months : No. of Months of Experience during Internships
  - certifications : No. of Certifications Completed
  - attendance_percentage : Percentage of Attendance Acheived during college
  - backlogs : No. of Backlogs accumulated during college
  - extracurricular_activities : Partipication in Extracurricular Activities
  - placement_status : Has Goten Placement
  - salary_package_lpa : Salary Package(LPA) if Got Placement
    
<img width="2260" height="901" alt="image" src="https://github.com/user-attachments/assets/2c23cc3c-98da-4c1a-9cec-647b6b8fa9e2" />
A snapshot of dataset
 

---

## 👥 Demographics Analysis
This section explores the background distribution of students.

**Gender-wise distribution of Students**

<p align="center">
  <img width="45%" alt="image" src="https://github.com/user-attachments/assets/91c76bea-0a24-4f2b-86e4-2110a8885c6d" />
  <img width="45%" alt="image" src="https://github.com/user-attachments/assets/a34953b2-9837-48b0-9341-7cac964c9d3e" />
</p>





With this visualization we can deduce that number of males is almost same as females, So The Data is Balanced and have perfect gender disparity.

**Visualizations Used:**
- Bar charts
- Pie / donut charts
  
---

## 📊 Academic Performance Analysis
Analysis of students’ academic outcomes.

**Analysis Focus:**
- CGPA / marks distribution
- Performance comparisons across groups

**Student distribution by Percentage Achieved in 10<sup>th</sup>/12<sup>th</sup>**<br>

<img width="1091" height="343" alt="image" src="https://github.com/user-attachments/assets/98454da7-7957-492f-9f0a-b12a8476f7b8" />
This Distribution dipicts that:
  
- consistent high performance: Whole Distribution follows a uniform distribution instead of having a Normal distribution(bell curve) and students are likely to score 95% as much likely for them to score 70%.
- Mojority of the Students are b/w 55% to 95%, acheiving a very healthy score portion.
- Normally Students Scored 55% and highest possible score of students is 95% and there is dip in scores in the middle resulting 60% is the least common score b/w students.
  
Moving on to,

<img width="1306" height="366" alt="image" src="https://github.com/user-attachments/assets/5932fc35-8f56-428e-975a-9e4cdfc64192" />

This Distribution dipicts that:
  
- Trend of Decline at the end: This distribution is more common to what we usualy find in scores distribution emerging as slightly positive skewed distribution ensuring achieving high score is more difficult.
-  Similar to previous Distribution, 55% is the Normally Achieved score within students and 95% is the highest achieved score.
-  Stablity of mid-Ranges Suggests that average performance are broad range plateau.


**Students Degree CGPA/Percentage Analysis**

<p align="center">
<img width="45%" alt="image" src="https://github.com/user-attachments/assets/6ede3a28-9bc0-4e7e-8d96-59b33523951c" />
<img width="45%" alt="image" src="https://github.com/user-attachments/assets/72ff7efb-b665-410b-bb36-cc650b3e3afa" />
</p>

According to the Distribution It Clears:

- Most Students Acheived High CGPA with 9.0 as the most common CGPA within students which only falls off at perfect 10.0 CGPA with 340 Students, This indicates a very strong overall academic performance.
- there are 7 students at 5.5 CGPA making that category a massive outlier, except that 99.8% students acheived more that 6.0 CGPA.
- Degree percentage Distribution follows a standard bell curve with clear boundaries of 56% and 89% with 71% in the middle as mean.



**Visualizations Used:**
- Histograms

---

## 🕒 Attendance Impact on Performance
Study of how attendance affects academic performance.

**Analysis Focus:**
- Attendance percentage vs CGPA
- Attendance grouped into categories (Low / Medium / High)
- Median CGPA across attendance groups

**Understanding impact of Attendance on CGPA**

Note: Y-Axis was truncated for the better view at the fluctuations.
<img width="1466" height="587" alt="image" src="https://github.com/user-attachments/assets/c8cc4706-8047-4463-ac56-b5ec0f084903" />
This Graph doesn't show any relation of attendance to CGPA at all:

- we expect that more attendance means more CGPA but that is not the case, its actually pretty stable to the point that difference b/w both minimas is less that 1 unit.
- Still we can see that, at 77% attendance there a peak of 8.2 Median CGPA suggest students with more 3 quarter attendance performs better that those with near perfect attendance suggesting balance of both class time and independent study or other activitites.
<br>
Because we couldn't uncover much relation between attendance and CGPA,

<img width="1004" height="613" alt="image" src="https://github.com/user-attachments/assets/cc509758-a616-45d9-9536-e263eb2e54cd" />

This Visualization tries a different approach, By creating different groups based on their attendance (<60%, <75%, >75%)

- At First, It seems that attendance has near to none effect on CGPA, because all of the groups has almost same numbers.
- But Low Group has only 133 samples in it which is only ~2.6% of the all students so we cant actually compare them to other groups.
- Apart from Low, Mid and High has compareable no. of students and it shows that More attendance justn't mean more CGPA.

**Techniques Used:**
- Feature binning
- Pivot tables

**Visualizations Used:**
- Line plots
- Box plots

---

## 🎯 Placement Analysis
Evaluation of placement outcomes and their drivers.

**Analysis Focus:**
- Overall placement rate
- Relationship between Different Features and Placement Status

**Placement Rate of Students**

<p align="center">
  <img width="45%" alt="image" src="https://github.com/user-attachments/assets/45c77289-67f1-42ce-9345-78489bb31a16" />
  <img width="45%" alt="image" src="https://github.com/user-attachments/assets/803004c7-9fa4-4497-b1a5-475495b6a229" />
</p>

Using This Visualization, We find

- There's a big amount of students weren't getting placed around 4150 to be exact which is a massive ~83% of all the students, Which Immediately signals Low Success Rate.
- To Can't investigate further without more context of Why only 17% students are getting Placed, Which can be is this data from the start of placement season or the end, if its the end of the season then 17% is alarming.
- Atleast We can Say that Both Gender are unsettled by this.

**Influence of Different Features on Placements**

<img width="1800" height="653" alt="image" src="https://github.com/user-attachments/assets/0bbcc0e2-7d09-482d-bc94-28d9b4adcf2a" />

According to this visualization, There is no fluctuations in line chart before 7.0 CGPA meaning,

- To have a better chance of placements, students needs to have atleast or more than 7.0 CGPA, or this could also mean that those with less than 7.0 CGPA aren't allowed for the interview.
- There are large peaks around 8.0 CGPA reaching even ~71% chances of placement.
- The Most Interesting Insight from this is that, everyone have almost same amount of chances of the placements meaning more CGPA doesn't grant a guarantee for placement, or it can't be the only factor responsible.

<img width="752" height="452" alt="image" src="https://github.com/user-attachments/assets/9d282fd8-4f75-4fdb-be11-8e032fed7458" />

With This Visualization we trying to find, does more attendance means better chances of placement. although there wasn't any coorelation b/w attendance % and placements, so we're apply the same thing as previous,

- Again As Low Attendance Group has a lot less no. of students, we can only compare the other two groups.
- Both Mid and High Attendance Groups has almost the same % of students placed, meaning High attendance doesn't mean better chances of placements.

Note: Y-Axis Was Truncated to see Variation Clearly.
<img width="1434" height="610" alt="image" src="https://github.com/user-attachments/assets/f38457ac-5474-4e86-ae48-580bac079dd2" />

Using this Chart We are trying to spot, Does Backlogs becomes a liability during Placements:

- On The First Glance We See, That After Those with more than 2 backlogs have 0% chance of placements, which could mean that either those with more than 2 backlogs aren't even allowed to take interview or there were just selected.
- There isn't much too see in the CGPA of students with different backlogs there isn't a big difference in CGPA, Which could just mean students are good in most of the subjects except some in which they have backlogs.
- Most amount of backlog, a student can have is 5 which means that there may be a creteria was applied on students with more than that.

<img width="1385" height="666" alt="image" src="https://github.com/user-attachments/assets/554c529d-fb8d-48aa-b374-a208fd19f4f6" />
Here We Applied a new Visualization which is a Scatter plot in Technical v/s Soft Skill with hue by placements. We already can see that, all the students with placements are always inside a specific range which is Technical Skill Should be more than 55 and Soft Skills Should be more than 60, To have a chance of placement.


<img width="1827" height="302" alt="image" src="https://github.com/user-attachments/assets/31429a88-c071-4bde-a707-54e0194be352" />

Here We Applied a Correlation B/w All of the Features, and found out that for placements there is a huge negative correlation with backlogs which we already Saw, then there are some other features with slightly positive correlation with placement like CGPA, Technical Skill Score and Soft Skill Score. So This Gives us a validation that all the results, We gathered were Correct and Liable.


**Visualizations Used:**
- Bar charts
- Stacked bar charts
- Pie charts
- Scatter plot

---

## 💰 Salary Insights
Analysis of compensation for placed students.

**Analysis Focus:**
- Salary distribution
- CGPA vs salary relationship

**Salary Distribution of Students**

<img width="1524" height="596" alt="image" src="https://github.com/user-attachments/assets/9a947e33-9929-4b3f-b3a1-234e4754a753" />

From This Visualization we can find out some things out:

- This Histogram is almost uniform, which is not normal to see because usually there are more students in between 3-4 LPA and lot less peoples at the high paying jobs but this histogram shows all salary jobs have almost same amount of students.
- Job with 15 LPA is the highest salary and it's also really common. As there are less number of students in 3-4 LPA jobs suggests college has a minimum required package given or Mass-Reqruiters are not allowed.


**Visualizations Used:**
- Histogram

---

## 📌 Key Findings & Recommendations
Summary of insights derived from the analysis.

**Examples:**
- Impact of attendance on academic performance
- Role of CGPA in placement probability
- Departments with strong placement outcomes

**Recommendations:**
- Actionable insights for students
- Suggestions for academic institutions

---

## 🛠 Tools & Technologies Used
- Excel / Google Sheets
- Python (Pandas, Matplotlib / Seaborn)
- Power BI / Tableau (if applicable)

---

## 📈 Future Improvements
- Add predictive modeling for placement outcomes
- Build an interactive dashboard
- Include time-series analysis across semesters

---

## 📎 Project Structure
