## School_District_Analysis
Project learning the use of Pandas


### In this challenge we learned how to analysis data using Pandas within Jupyter notebook. Using some of the similar code writing skills that we learned during the last project and applying that skill to this one. We learned how to filter what we want from the data, drop what we don’t need, and how get calculate the sum, mean, counts, etc. 

### In this analysis we processed data that was provided for 15 different high schools within a district. Some of the information we collected was the differences in scores between the public and charter schools. The charter schools had slightly better scores with it came to math and reading than the scores within public schools. We further broke down those scores to shows us the difference between public and charter school via each grade level. For the most part charter schools scores were higher in all grades except for 12th grade [1]. 
![student data image 1](https://user-images.githubusercontent.com/112769590/194457292-95ec8a4e-0e19-49fe-b1d5-ee3eb83c5e9c.png)
![student data image 2](https://user-images.githubusercontent.com/112769590/194457293-d888850b-bbff-48af-b9af-e94d873ea67b.png)



### We were also able to determine the total number of students that attended each school but counting the ID’s for each student. We did this but using a groupby formula; student_count = student_df.groupby(by='school_name').count() and we displayed the results of that data using the formula; student_count.loc[:, ["student_id"]]. [1]
![student data image 4](https://user-images.githubusercontent.com/112769590/194457327-861d114b-9338-434a-aaac-08aee4ea3839.png)


### When an anaylest of the data was first ran we saw a few of the results yielded the value “NaN” this let us know that data was possibility missing or incorrectly input. We learned how to count of the amount of data that have a “NaN” value and drop or edit the results so that it would not have a significant impact on our findings [2]. For this project we found that there was a combined 2950 items of data missing by using the formula; student_df.isnull().sum(). We determined it would be best to drop that missing data rather than replacing it with another value using formula; student_df = student_df.dropna() [1].
![student data image 3](https://user-images.githubusercontent.com/112769590/194457339-c17a0be7-f4e1-467f-a005-5ce09d4e2165.png)



#### [1] Jupyter notebook folder: School_District_ Analysis – file: Challenge_New_Student_Data
#### [2] 4.3.2 Handling Missing Data
