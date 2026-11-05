# Password Requirements Display
US1 – Account Creation

### Metrics
Adoption Rate: Firebase Authentication (Track the percentage of users who successfully create an account) and Firebase Analytics (Track successful account creations and password validation errors).

### Hypothesis
Some GarageLink users may struggle to create an account because they don't know the password requirements until they get an error. Displaying the password requirements before users enter their password may reduce errors and make account creation easier. We hypothesize that showing password requirements will increase successful account creations and reduce password errors.

### Experiment
We will use Firebase A/B Testing and Remote Config to test two versions of the GarageLink sign-up page. 50% of new users will see Variation A, and 50% will see Variation B. Firebase Analytics will track successful account creations, password validation errors, and the number of users who start the sign-up process. We will compare the results to determine whether displaying password requirements improves account creation.

### Variations
Variation A – No Password Requirements Display
Users enter their password without seeing the requirements beforehand. If their password does not meet the requirements, an error message appears.

Variation B – Password Requirements Display
Users see the password requirements directly below the password field before entering their password.

---

# One tap login
US2 - User Login

### Metrics
Primary Metric: Sign-In Conversion Rate. Measure the percentage of users who successfully sign in after viewing the login page. Secondary Metrics: Number of clicks on each sign-in option. Percentage of users who begin the sign-in process but do not complete it. Time it takes users to successfully sign in. Number of users who successfully create an account. These metrics will help determine which login method is easier and more effective for users.

### Hypothesis
I believe that users will be more likely to sign in using one-tap authentication options, such as Google or Apple, rather than entering their email address and password manually. By providing faster sign-in options, we expect to reduce the effort required to access the app and increase the number of users who successfully sign in.

### What problem are we trying to solve?
Users today often expect applications to provide quick and convenient ways to access their accounts. Traditional email and password login requires users to manually enter their credentials, which can take additional time and effort. This extra effort may discourage users from signing in or cause them to abandon the process. For garagelink, we want to make signing in as simple and convenient as possible. By offering one-tap authentication options, we hope to reduce the time users spend logging in and allow them to access the app's features more quickly.

### Experiment 
We will use Firebase A/B Testing and Firebase Analytics to compare two different login page designs Users will be randomly assigned to one of the two variations. Each user will continue to see the same variation during the experiment to ensure a consistent experience. 

### Variations
Traditional Login - The login page will contain: Email address field, Password field, Sign-in button, Sign-up option. This represents the traditional email and password login experience. Variation B — One-Tap Login - The login page will contain: Google sign-in button, Apple sign-in button, Email and password login option, Sign-up option, This variation introduces additional one-tap sign-in options while keeping traditional login available.

---

# Profile Setup – Required or Skip for now
US3 - Profile Creation

### Metrics
- Adoption: percent of new sign ups who make it to homepage using Firebase Authentication and Analytics
- Task Success: percent of new users with a finished profile after a week using Firebase Analytics

### Hypothesis
New users are forced to fill out their profile as soon as they create an account. This is the first thing they see so if it feels like too much, they might close the app and delete. This is where we expect users to drop off and it hurts us because every user we lose is one less person buying or selling parts. If we let new users skip profile setup and come back to it later, more of them will reach the homepage and most will still end up finishing their profile.

### Experiment
- Tool: Firebase A/B Testing with Remote Config that turns the skip button on or off
- Audience: new users only (current users already have a profile) split 50/50 into two groups
- Tracking: Firebase Analytics to track how many users skip profile setup, finish their profile (Task Success), and reach the homepage (Adoption)
- Success: Version B wins if more users reach the homepage and the finished profile rate stays the same after a week

### Variations
- Version A (current): After sign up users cant leave profile page until picture, name, username, and car are filled in
- Version B: same profile page, plus a "Skip for now" under the Save button. Skipping goes straight to the homepage

---

# Filter Usage Rate (Side Panel or Top Panel)
US4 - Golden Path 

### Metrics
Engagement: the filter usage rate which is a combination of how much it is opened and how often the home page is viewed  

### Hypothesis
The issue is that buyers drop off between the home feed and filtering because the filter is hidden. I believe that testing where the  filter is placed may impact the likliness of the buyer using it. This would lead to more accurate searches and thus more frequent purchases from users.

### Experiment 
- A Firebase Remote Config Parameter, filterLayout, will split the users 50/50 through firebase A/B testing

- Only users who reach the home page are counted towards this test

- Our hypothesis is that having a filter at the top of the screen with labeled buttons (ie. Price, Condition, Make/Model) will help increase filter usage. Filter placement is the only thing that changes between the two versions.
  
### Variations

Variation A: Top Filters
A row of labeled chips under the search bar (Category, Price, Condition, Make/Model, Distance) that scroll sideways. Tapping on a chip will open that filters options in a bottom sheet.

Version B Side Panel
One filter icon next to the search bar. By tapping on it, it will slide a panel from the side with every filter listed as well as Apply and Clear buttons.

---

# Tile item listings on wider monitors instead of one per row
US# - 

### Metrics
Engagement: Track how long users scroll through listings and how many listings they interact with
Retention: Track how frequently users with wider displays return to the app

### Hypothesis
The amount of dead space on wider screens may be inconvenient for users, as the information is spread farther apart, and people spend longer scrolling.

### Experiment
A firebase remote config parameter, create two versions of the page, and use analytics to see how fast users navigate to a listing page.

### Variations

Variation A: One item per row, with details spread to fill screen

Variation B: Multiple items per row, with each individual item n

---

