# Detectecting_Heart_Disease-SVM
### **Task:** Detecting Heart disease in patients using SVM

### **Trained Model:** Accuracy: 100%
### **Dataset available on:** [UCI Machine Learning Heart Disease](https://archive.ics.uci.edu/dataset/45/heart+disease) , [Kaggle](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)

**Developers' Guide:** [Amazon Machine Learning](https://docs.aws.amazon.com/pdfs/machine-learning/latest/dg/machinelearning-dg.pdf#cross-validation)                                             
**Link to the notebook:** [Heart-Disease-SVM](https://github.com/Kmohamedalie/Detectecting_Heart_Disease-SVM/blob/master/Notebook/Heart_Disease_SVM.ipynb)


![image](https://github.com/Kmohamedalie/Detectecting_Heart_Disease-SVM/assets/63104472/d37d60ff-f208-4626-85c9-9db85582b83f)

### **Publication Request:**
   >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
   This file describes the contents of the heart-disease directory.

   This directory contains 4 databases concerning heart disease diagnosis.
   All attributes are numeric-valued.  The data was collected from the
   four following locations:

     1. Cleveland Clinic Foundation (cleveland.data)
     2. Hungarian Institute of Cardiology, Budapest (hungarian.data)
     3. V.A. Medical Center, Long Beach, CA (long-beach-va.data)
     4. University Hospital, Zurich, Switzerland (switzerland.data)

   Each database has the same instance format.  While the databases have 76
   raw attributes, only 14 of them are actually used.  Thus I've taken the
   liberty of making 2 copies of each database: one with all the attributes
   and 1 with the 14 attributes actually used in past experiments.

   The authors of the databases have requested:

      ...that any publications resulting from the use of the data include the 
      names of the principal investigator responsible for the data collection
      at each institution.  They would be:

       1. Hungarian Institute of Cardiology. Budapest: Andras Janosi, M.D.
       2. University Hospital, Zurich, Switzerland: William Steinbrunn, M.D.
       3. University Hospital, Basel, Switzerland: Matthias Pfisterer, M.D.
       4. V.A. Medical Center, Long Beach and Cleveland Clinic Foundation:
	  Robert Detrano, M.D., Ph.D.

   Thanks in advance for abiding by this request.

   David Aha
   July 22, 1988
   >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

1. Title: Heart Disease Databases

2. Source Information:
   (a) Creators: 
       -- 1. Hungarian Institute of Cardiology. Budapest: Andras Janosi, M.D.
       -- 2. University Hospital, Zurich, Switzerland: William Steinbrunn, M.D.
       -- 3. University Hospital, Basel, Switzerland: Matthias Pfisterer, M.D.
       -- 4. V.A. Medical Center, Long Beach and Cleveland Clinic Foundation:
             Robert Detrano, M.D., Ph.D.
   (b) Donor: David W. Aha (aha@ics.uci.edu) (714) 856-8779   
   (c) Date: July, 1988

3. Past Usage:
    1. Detrano,~R., Janosi,~A., Steinbrunn,~W., Pfisterer,~M., Schmid,~J.,
       Sandhu,~S., Guppy,~K., Lee,~S., \& Froelicher,~V. (1989).  {\it 
       International application of a new probability algorithm for the 
       diagnosis of coronary artery disease.}  {\it American Journal of 
       Cardiology}, {\it 64},304--310.
       -- International Probability Analysis 
       -- Address: Robert Detrano, M.D.
                   Cardiology 111-C
                   V.A. Medical Center
                   5901 E. 7th Street
                   Long Beach, CA 90028
       -- Results in percent accuracy: (for 0.5 probability threshold)
             Data Name:  CDF    CADENZA
          -- Hungarian   77     74
             Long beach  79     77
             Swiss       81     81
          -- Approximately a 77% correct classification accuracy with a
             logistic-regression-derived discriminant function
    2. David W. Aha & Dennis Kibler
       -- 
          
          
          -- Instance-based prediction of heart-disease presence with the 
             Cleveland database
             -- NTgrowth: 77.0% accuracy
             --       C4: 74.8% accuracy
    3. John Gennari
       -- Gennari, J.~H., Langley, P, \& Fisher, D. (1989). Models of
          incremental concept formation. {\it Artificial Intelligence, 40},
          11--61.
       -- Results: 
          -- The CLASSIT conceptual clustering system achieved a 78.9% accuracy
             on the Cleveland database.

4. Relevant Information:
     This database contains 76 attributes, but all published experiments
     refer to using a subset of 14 of them.  In particular, the Cleveland
     database is the only one that has been used by ML researchers to 
     this date.  The "goal" field refers to the presence of heart disease
     in the patient.  It is integer valued from 0 (no presence) to 4.
     Experiments with the Cleveland database have concentrated on simply
     attempting to distinguish presence (values 1,2,3,4) from absence (value
     0).  
   
     The names and social security numbers of the patients were recently 
     removed from the database, replaced with dummy values.

     One file has been "processed", that one containing the Cleveland 
     database.  All four unprocessed files also exist in this directory.
    
5. Number of Instances: 
        Database:    # of instances:
          Cleveland: 303
          Hungarian: 294
        Switzerland: 123
      Long Beach VA: 200

6. Number of Attributes: 76 (including the predicted attribute)

7. Attribute Information:
   -- Only 14 used
      -- 1. #3  (age)       
      -- 2. #4  (sex)       
      -- 3. #9  (cp)        
      -- 4. #10 (trestbps)  
      -- 5. #12 (chol)      
      -- 6. #16 (fbs)       
      -- 7. #19 (restecg)   
      -- 8. #32 (thalach)   
      -- 9. #38 (exang)     
      -- 10. #40 (oldpeak)   
      -- 11. #41 (slope)     
      -- 12. #44 (ca)        
      -- 13. #51 (thal)      
      -- 14. #58 (num)       (the predicted attribute)

   -- Complete attribute documentation:
     
9. Missing Attribute Values: Several.  Distinguished with value -9.0.

10. Class Distribution:<br>

| Database:    |    0    |    1    |    2    |    3    |    4    |    Total  |
| ------------ | --------| --------| --------| --------| --------| ----------|
|Cleveland:    |   164   |   55    |   36    |    35   |    13   |     303   |
|Hungarian:    |   188   |   37    |   26    |    28   |    15   |     294   |
|Switzerland:  |     8   |   48    |   32    |    30   |    5    |     123   |
|Long Beach VA:|    51   |   56    |   41    |    42   |    10   |     200   |
