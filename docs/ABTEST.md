A/B Test Name:  login In 1 button or the old fashion email and password
## A/B Test Name: 

## User Story Number:

## Metrics: 

## Hypothesis:

## Experiment:

## Variations: 



## A/B Test Name: Password Requirements Display

## User Story Number: US1 – Account Creation

## Metrics: Adoption Rate: Firebase Authentication (Track the percentage of users who successfully create an account) and Firebase Analytics (Track successful account creations and password validation errors).

## Hypothesis: Some GarageLink users may struggle to create an account because they don't know the password requirements until they get an error. Displaying the password requirements before users enter their password may reduce errors and make account creation easier. We hypothesize that showing password requirements will increase successful account creations and reduce password errors.

## Experiment: We will use Firebase A/B Testing and Remote Config to test two versions of the GarageLink sign-up page. 50% of new users will see Variation A, and 50% will see Variation B. Firebase Analytics will track successful account creations, password validation errors, and the number of users who start the sign-up process. We will compare the results to determine whether displaying password requirements improves account creation.

## Variations:
Variation A – No Password Requirements Display
Users enter their password without seeing the requirements beforehand. If their password does not meet the requirements, an error message appears.
Variation B – Password Requirements Display
Users see the password requirements directly below the password field before entering their password.




## A/B Test Name: 

## User Story Number:

## Metrics: 

## Hypothesis:

## Experiment:

## Variations: 


## A/B Test Name: 

## User Story Number:

## Metrics: 

## Hypothesis:

## Experiment:

## Variations: 


## A/B Test Name: 

## User Story Number:

## Metrics: 

## Hypothesis:

## Experiment:

## Variations: 



User Story Number: US1

Metrics: Primary Metric: Sign-In Conversion Rate. Measure the percentage of users who successfully sign in after viewing the login page. Secondary Metrics: Number of clicks on each sign-in option. Percentage of users who begin the sign-in process but do not complete it. Time it takes users to successfully sign in. Number of users who successfully create an account. These metrics will help determine which login method is easier and more effective for users.

Hypothesis: I believe that users will be more likely to sign in using one-tap authentication options, such as Google or Apple, rather than entering their email address and password manually. By providing faster sign-in options, we expect to reduce the effort required to access the app and increase the number of users who successfully sign in.

What problem are we trying to solve? Users today often expect applications to provide quick and convenient ways to access their accounts. Traditional email and password login requires users to manually enter their credentials, which can take additional time and effort. This extra effort may discourage users from signing in or cause them to abandon the process. For garagelink, we want to make signing in as simple and convenient as possible. By offering one-tap authentication options, we hope to reduce the time users spend logging in and allow them to access the app's features more quickly.

Experiment - We will use Firebase A/B Testing and Firebase Analytics to compare two different login page designs Users will be randomly assigned to one of the two variations. Each user will continue to see the same variation during the experiment to ensure a consistent experience. 

Variations - Traditional Login - The login page will contain: Email address field, Password field, Sign-in button, Sign-up option. This represents the traditional email and password login experience. Variation B — One-Tap Login - The login page will contain: Google sign-in button, Apple sign-in button, Email and password login option, Sign-up option, This variation introduces additional one-tap sign-in options while keeping traditional login available.
