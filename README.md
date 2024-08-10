![](https://github.com/Adeyemi0/User-Journey-Analysis/cj.jpg)

## Introduction
The goal of this project is to analyze the user journey data from a subscription-based platform to uncover insights that can inform strategic decisions aimed at improving conversion rates and reducing user churn. This project focuses on examining the paths users take as they navigate through various pages on the platform, from the initial landing page to key conversion points such as sign-up, log-in, and checkout. By analyzing patterns in both converting and non-converting journeys, we aim to identify the factors that contribute to successful conversions as well as the barriers that lead to user drop-off.

### Dataset Description
#### Source
The data was collected from website user logs, tracking user interactions and journeys through various pages.
Content
The dataset comprises 9,935 entries, detailing user interactions and journeys. Number of users are 1,350. It includes:
*	user_id: Unique identifier for each user.
*	session_id: Identifier for each session.
*	subscription_type: Type of subscription (e.g., annual, monthly).
*	user_journey: The sequence of pages visited by users.

### Data Preprocessing
#### Key Columns Added
*	cleaned_journey: The sequence of pages visited by users.
*	is_converted: A binary indicator of whether the user converted.
*	num_pages: The number of pages a user visits during a session on the website.
*	journey_length: The number of steps in a user's journey.

## INSIGHTS
### Insights from Non-Converting Journeys
#### Top Non-Converting Journeys:

*	Log in (2,257 occurrences): The most common non-converting journey involves users repeatedly logging in without progressing further in the conversion funnel. This suggests that while users are engaging with the platform, they are not finding a compelling reason or sufficient guidance to move towards a purchase or checkout.
*	Other (1,012 occurrences): The 'Other' category is the second most common non-converting path. This broad category likely includes a variety of user actions that do not align with the main
conversion steps. This could indicate a lack of focus or clarity in the user experience, leading to disengagement.
*	Coupon (1,003 occurrences): A significant number of users interact with coupons but do not proceed to checkout. This could point to issues with coupon validity, application, or a mismatch between coupon expectations and actual discounts offered.
*	Homepage-Log in (849 occurrences): Users who begin at the homepage and log in but do not proceed further could be existing users who are not finding value in the subsequent steps or new users who lose interest after logging in.
*	Homepage-Sign up (202 occurrences): Users starting from the homepage and signing up but not converting suggests that while the initial engagement is successful, the follow-through is lacking, potentially due to onboarding issues or unmet expectations post-sign-up.

### Insights from Converting Journeys
#### Top Converting Journeys:
*	Checkout (1,773 occurrences): The most common converting path is straightforward, with users heading directly to checkout. This indicates that these users have already made a decision and are likely repeat customers or those who found what they needed quickly.
*	Pricing-Checkout (70 occurrences): A significant number of users who check the pricing page proceed to checkout, highlighting the importance of clear, attractive pricing information in driving conversions.
*	Homepage-Pricing-Checkout (60 occurrences): Users who navigate from the homepage to pricing and then to checkout show a more deliberate decision-making process. These users likely needed to evaluate the cost before committing.
*	Courses-Pricing-Checkout (6 occurrences): This path, though less frequent, shows that some users who explore course options before checking pricing still convert, indicating that course offerings are a factor in their purchase decisions.
*	Homepage-Pricing-Checkout-Homepage-Log in (4 occurrences): This journey, while rare, suggests a more complex decision-making process, possibly involving returning users or those who needed to log in to apply a discount or check their account before completing the purchase

### Churn Transition Analysis
#### Key Churn Transitions:
*	Homepage to Log in (912 transitions): This is the most common transition, indicating that a significant number of users log in without proceeding further. This could represent returning users who are not sufficiently re-engaged upon logging in.
*	Homepage to Sign up (329 transitions): Many users begin signing up but do not complete the conversion. This might suggest a drop-off during or after the sign-up process.
*	Homepage to Pricing (307 transitions): Users who navigate from the homepage to the pricing page are considering a purchase but may not find the pricing compelling enough to continue.
*	Homepage to Career tracks (280 transitions): Users exploring career tracks from the homepage indicate interest in specific content areas but may not find a direct path to conversion.
*	Career tracks to Courses (265 transitions): Users moving from career tracks to courses suggest that while there is interest in content, it does not necessarily translate into conversions, perhaps due to unclear value propositions or pricing.

### Session Length Analysis
The average session length is 1.70 pages, indicating that most users are not deeply exploring the site. This relatively short session length suggests that users either find what they need quickly (in the case of converting users) or do not engage deeply enough to convert (in the case of non-converting users).

## RECOMMENDATION
1.	Enhance the Onboarding Process:
Simplify Sign-Up and Log-In: Streamline the sign-up and log-in processes to ensure that users can move quickly from these steps into more valuable interactions. Consider implementing guided walkthroughs or tooltips to help new users navigate the platform more effectively.

Improve Post-Login Engagement: For users who log in without converting, provide personalized content or offers that could nudge them towards conversion, such as reminders of items left in their cart or special discounts.

2.	Revamp the Pricing Page:
Clearer Value Propositions: Ensure that the pricing page clearly communicates the value users receive for each pricing tier. Include testimonials, case studies, or specific benefits to make the pricing more compelling.

Simplify Coupon Application: Address any potential issues with coupon application to ensure users can easily apply discounts without frustration. Consider A/B testing different coupon presentations to see which drives higher conversions.

3.	Focus on Retargeting Non-Converting Users:
Targeted Campaigns: Use retargeting strategies to bring back users who frequently log in without converting. Personalized emails or ads that address their specific behaviors on the site (e.g., viewed pricing but didn’t purchase) could be effective.

## LIMITATIONS OF THE DATASET
1.	The lack of timestamp data limits the ability to perform true recency and churn analyses.
2.	The data does not differentiate between types of users (e.g., new vs. returning), which could provide deeper insights into behavior patterns.








