# MechaCar Statistical Analysis:

Analysis of MechaCar prototypes (mpg, psi, manufacturing lots, and vehicle performance).

## Linear Regression to Predict MPG

- The vehicle length and ground clearance have a significant (non-random) impact on the variance of the mgp.
  
- The slope or this linear model is not zero. A small p-value (typically ≤ 0.05) indicates strong evidence against the null hypothesis (that the slope is equal to zero). Since the p-value here is extremely small (5.35e-11), it is safe to say that the slope is not zero.
  
- This linear model predicts mpg of MechaCar prototypes effectively. We know this because of the Multiple R-squared value of 0.7149. This means that it will predict the mpg correctly 71% of the time.

## Statistical Summary:

<img width="491" alt="image" src="https://user-images.githubusercontent.com/106691255/201000455-8a7b4ce2-da71-44e9-9721-0eeebc9b8057.png">

## Summary Statistics on Suspension Coils:

### Total Summary:

<img width="337" alt="image" src="https://user-images.githubusercontent.com/106691255/201004421-4e3030a6-2f3f-4ee2-a315-db4fcf69274a.png">

### Lot Summary: 

<img width="490" alt="image" src="https://user-images.githubusercontent.com/106691255/201004504-1173ddd2-b9ec-4496-9250-4196c9aaf18b.png">

- The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch.   * The current manufacturing data meets this design specification for all manufacturing lots in total. The PSI Variance in total is 62 which is well below the 100 PSI that is dictated.
  * Lots 1 and 2 have variances of 0.9795918 and 7.4693878 respectivly, which are also well within the 100 PSI range.
  * Lot 3, however, has a variance of 170.2861224, which is too far above the 100 PSI specification.

## T-Test on Suspension Coils:

### Interpretation and findings for the T-Test results:

- There was a presumed population mean of 1500 for the sample. Through the t-test, it was determined that the true mean of the entire set was 1498.78.
  * Lot 1: Mean of 1500, P-Value of 1 - This lot is statistically similar to the presumed population.
  * Lot 2: Mean of 1500.2, P-Value of 0.6072 - This lot is also statistically similar to the presumed population.
  * Lot 3: Mean of 1496.14, P-Value of 0.04168 - This lot is NOT similar to the presumed population. The null hypothesis can be rejected. Something went awry with the production of this lot and it should be put under investigation.

#### T-Test for Entire Set
<img width="414" alt="image" src="https://user-images.githubusercontent.com/106691255/201005316-64fc69ef-d74e-4291-b292-06d5d6c822c2.png">

#### T-Tests for Each Lot:
<img width="406" alt="image" src="https://user-images.githubusercontent.com/106691255/201005437-f64c3767-2785-4bb2-ae0a-a26f304287fa.png">

## Design a Study Comparing the MechaCar to the Competition

Another study that MechaCar could do is safety ratings.

- The metrics that I am going to test are:
  * Frontal crash test
  * Side crash test
  * Rollover resistance test
  * Head restraint and seat tests
  * Roof strength test
- The null hypothesis states that the safety rating is equal to zero, and the alternative hypothesis states that the safety rating is not equal to zero.
- To test the hypothesis, I would use a t-test because it would determine if the means between MechaChar and its competitors are statistically similar or not.
- The data needed to run the above test would be a random sampling of data from MechaCar and its competitor using the above metrics.
