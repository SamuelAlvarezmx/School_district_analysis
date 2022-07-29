# School District Analysis
 ## Overview

 This analysis was performed to illustrate to the school board of directors how is the performance of different schools and how does the type, size and budget have any trend in the performance of their students. Also it was needed to clean the data that was given becuase there were prefixes and suffixes in the names of some students and also there was a case of academic dishonesty, therefore it was needed to change and ignore some of the starting information. The school board of directors asked for a comparison in how does the analysis changed when the school and students in which the academic dishonesty was found were not considered in this assessment.

 ## Results

 During the exercise of dropping the ninth graders' scores, Thomas High School´s performance was seriously impacted. However, when we modified the reference and only used the 10th to 12th grade students, the performance didn´t changed as dramatically as it looked at first glance. In the following lines the results of the analysis will be discussed

 * **How is the district summary affected?**

   The district summary according to the rounding of the numbers to one decimal point is not affected or at least it can be perceived, therefore no change can be reported in this area

  ![district_summary](https://user-images.githubusercontent.com/104656920/181684627-3741398b-b8c9-4d91-950e-64ed70d1fd9e.png)


  * **How is the school summary affected?**

   1. The school summary was one of the more affected DataFrames when talking about the scores for the Thomas High School. As shown in the below image, the Overall passing was at firt 90.948% This data point was considerin all the students and considering the ninth graders.

  ![per_school_summary](https://user-images.githubusercontent.com/104656920/181684692-12870cd2-76b4-4eaf-bf6a-8ce6e41facef.png)


   2. However, when analyzed the data dropping down the ninth graders scores and considering the whole students in Thomas High School, the scores went down in a very notorious way as shown in the below image
   ![per_school_summary_challenge](https://user-images.githubusercontent.com/104656920/181684727-f5f90f26-29ce-4428-b4b8-2c0b9979f336.png)


   3. The later analysis is not correct because we cannot consider the students that have no longer a score in math and reading, therefore making the change of the total students in Thomas High School to not consider the ninth graders, we get the school_summary closer to what the school performed counting the ninth graders. The % Overall passing went from 65.076% to 90.630%. Compared to the beginning summary, we are only perceiving a 0.3% change in our results.

   ![per_school_summary_challenge_1](https://user-images.githubusercontent.com/104656920/181684736-01ae3da3-74ae-4d5b-bfe6-9cf76651e9f2.png)

   * **How does the replacing the ninth grade scores affect the following:**

     It can not be perceived an impact on all of the assessed fields, at least not with the sensibility of representative numbers that the analysis was asked to be done.

     * Math and reading scores
     ![Math_scores](https://user-images.githubusercontent.com/104656920/181684775-3b1927ae-1dc7-4b44-a6b0-df1ec30a3c75.png)
 ![reading_scores](https://user-images.githubusercontent.com/104656920/181684785-ebbd9ecb-0be1-49d8-89e1-b004c6578b2a.png)


     * Scores by school spending

     ![spending](https://user-images.githubusercontent.com/104656920/181684830-614d654e-f3aa-485c-8909-d1d97c459a3d.png)

     * Scores by school size

     ![school_size](https://user-images.githubusercontent.com/104656920/181684818-7a8f7845-9bdc-43bb-b495-5a38cccb89ee.png)

     * Scores by school type
     ![school_type](https://user-images.githubusercontent.com/104656920/181684807-2347fed8-276f-44b2-acda-a1d11a148d0f.png)


 ## Summary

   After reviewing the new dataset with the modifications asked by the school board of directors, the findings on how these changes affected our analysis can be mentioned.

   * The overall passing changed a bit for Thomas High scholl, however, this change is not relevant because after fixing the student number, the averages were very similar to what was seen in the first analysis.

   * If we do not consider the ninth graders scores but do take into account the number of ninth graders, we could make a mistake in presenting the analysis, because we are assuming that everyone just scored 0 in the assignments, which can completely ruin our objective analysis.

   * When looking for the scores of all the students in the district, there will be NaN values, indicating the lack of data

   * Considering that there was academic dishonesty, the other students from grades above, do have a high performance because considering just those students, Thomas High School continues to be the second school in the top five of performance.
