
## Dataset

This dataset collects information from 100k medical appointments in Brazil and is focused on the question of whether or not patients show up for their appointment. A number of characteristics about the patient are included in each row.

-‘ScheduledDay’ tells us on what day the patient set up their appointment. -‘Neighborhood’ indicates the location of the hospital. -‘Scholarship’ indicates whether or not the patient is enrolled in Brasilian welfare program Bolsa Família. -'No-show' indicates whether or not the patients showed up for their appointment.

-Under 'No-show', ‘No’ indicates that patient showed up to their appointment, and ‘Yes’ indicates that they did not show up.

-Under 'Scholarship' and other characteristics, '0' indicates that it is true for the patients and '1' indicates that it is false.

## Findings

The aim of this analysis was to answer two important research questions.

Question 1: Important factors to consider inorder to predict if patients will show up for their scheduled appointment.

Question 2: Influence of diseases and disability on enrollment for welfare program (Scholarship)

The data was found to be devoid of duplication and also had no null value. It was however found that some of the patients had ages zero (0), which could not be true. So such datas of patients with ages zero was dropped.

The dataset was categorised based on those that showed up for appointment and those that did not show up, and necessary correlations were made and visualized.

Findings revealed that enrollment for welfare program was an important factor that influenced patients showing up for appointment. This may be due to the benefit of reduction in the cost of care from the patient's end. Also, patients with one or two disease/disability and those that received SMS showed up more for appointment.

Equally, analysis result established that majority of patients enrolled for the welfare program had one or two diseases and disability. Likewise, majority of those enrolled for the welfare program were non-alcoholic patients.

## Insights

1. Scholarship (enrollment into welfare program) had a influence on Patients showing up for appointments.
2. SMS played a positive role in influencing patients to show up for appointments.
3. Data investigation established that more patients with one or mulitple types of disease showed up for their appointment. Diagnosis was therefore an important factor that influenced patients showing up for appointment.
4. More patients with Hypertension were enrolled in the welfare program.
5. More patients with Diabetes were also enrolled in the welfare program as opposed to the non diabetic patients.
6. More of non alcoholic patients were enrolled in the welfare program as opposed to alcoholic patients.
7. Majority of patients who enrolled for the welfare program had one or two diseases.
8. Most patients who showed up for appointment had diseases or disability and were enrolled in the welfare program.
9. More of the hypertensive patients that showed up for their appointment were enrolled in the welfare program.
10. More of the diabetic patients that showed up for their appointment were enrolled in the welfare program.
11. More of the sponsored patients that showed up for their appointment were non-Alcoholic patients. This implies that less Alcoholic patients were not sponsored.
12. Most patients who did not show up for appointment also had diseases and were equally enrolled in the welfare program.
13. More of hypertensive patients that refused to show up for appointment were enrolled in the welfare program.
14. More of diabetic patients that refused to show up for appointment were enrolled in the welfare program.
15. More of alcoholic patients that refused to show up for appointment were not enrolled in the welfare program.
