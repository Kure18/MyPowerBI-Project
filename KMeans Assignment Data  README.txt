# KMeans Assignment Data Dasboard

### Problem Statement
-To find the number of students that accepted the application but refused to enroll and the percentage of students that accepted the admission
-To find the difference between the number of students that made applications to those that enrolled at the end of the process
-To  find the total number of undergraduates

Steps 1-I created the following columns using DAX expressions:
        refused_enrol = Kmeans_assignment_data[Accept]-Kmeans_assignment_data[Enrol]
        overall_%_accepted = {Kmeans_assignment_data[Accept]/Kmeans_assignment_data[Apps]}*100
        Apps_Enrol = Kmeans_assignment_data[Apps]-Kmeans_assignment_data[Enrol]
        Total_undergrad = Kmeans_assignment_data[P.Undergrad]+Kmeans_assignment_data[F.Undergrad]
       
      2-Created a line chart with x="Accept", y="Sum of P.Undergrad" and "Sum of F.Undergrad"
      3-A scattered plot was created with x="Sum of Accept" and y ="Sum of refused_enrol" with values="P.Undergrad",
        "P.Undergrad"
      4-An area chart was created with x="Total_Undergrad", y="Sum of P.Undergrad", "Sum of F.Undergrad"
      5-Clustered column chart was created with x="Accept", y="Sum of F.Undergrad", "Sum of PhD", "Sum of P.Undergrad" with the highest value at 31.6k 
      6-100% stacked column chart was created
      7-A card was created displaying the "Sum of undergrad"



