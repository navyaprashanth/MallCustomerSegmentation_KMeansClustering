# Mall Customer Segmentation using K-Means Clustering
This project applies the K-Means Clustering algorithm to segment mall customers based on their purchasing and income habits. The goal is to identify distinct customer groups for targeted marketing strategies.

## Dataset
Source: [Mall Customer Data](https://github.com/navyaprashanth/MallCustomerSegmentation_KMeansClustering/issues/1#issue-3624804304)

File: [Mall_Customers.csv](https://github.com/user-attachments/files/23544206/Mall_Customers.csv)

## Project Breakdown
### 1. Data loading and cleaning
We load the data using Pandas and perform a basic check for missing values.

### 2. Feature Selection
We isolate the two columns critical for clustering: Annual Income (column index 3) and Spending Score (column index 4).

### 3. Determining the Optimal Number of Clusters (K)
The Elbow Method is used to find the ideal number of clusters by minimizing the Within Cluster Sum of Squares (WCSS). We test K from 1 to 10.

### 4. Visualizing the Elbow Graph
The plot shows the point where the decrease in WCSS starts to slow down significantly (the "elbow" which I have marked with a red dot in the graph).

<img width="610" height="463" alt="Image" src="https://github.com/user-attachments/assets/71bae946-86e7-4bd1-a2a2-ed98df3c5e36" />

The optimal number is 5 over here. 

### 5. Training the Model
We train the K-Means model using the optimal K =5

### 6. Visualizing the Clusters
The final plot shows the 5 resulting customer groups, with the cyan points representing the cluster centroids.
<img width="705" height="710" alt="Image" src="https://github.com/user-attachments/assets/7626b3a5-db00-4ee8-8ebc-7e153cbbb6fe" />

### Interpretation
<img width="706" height="180" alt="Image" src="https://github.com/user-attachments/assets/99600c67-e0b3-4e8f-9892-9f54e863c4bc" />

### Strategies
Keeping in mind this segmentation, effective strategies can be implemented to reach organisational goals such as:
1. Red cluster:

a. Offer an exclusive, tiered loyalty program (e.g., a "Platinum Club") with dedicated parking, private shopping hours, and early access to sales.

b. Personalization: Use their purchase history to send highly personalized, high-value recommendations (e.g., an invitation to a private event for a luxury brand they frequently buy).

c. Retention: Focus heavily on retaining them, as losing one of these customers significantly impacts revenue.


2. Blue cluster:

a. High-Volume Promotions: Market frequent, exciting sales, flash deals, and BOGO (Buy One Get One) offers for clothing, entertainment, and fast-moving consumer goods.

b. Credit/Financing: Promote payment plans or store credit cards to facilitate their desire to spend (focusing on things they can't afford at the moment but want to as that will make them look expensive).

c. Social & Entertainment Focus: Highlight affordable entertainment options like food courts, arcades, or budget-friendly movie deals, as they use the mall more for experiences.

3. Green cluster:

a. Consistency: Focus on broad, generic promotions that appeal to the mass market, such as seasonal sales (Back-to-School, Holiday).

b Convenience: Ensure the basic shopping experience (parking, store layout, services) is smooth and efficient to keep them coming back.

c. Upselling: Use targeted digital ads to introduce them to slightly higher-priced items than they typically buy, aiming for gradual increase in spending.

4. Yellow cluster:

a. Value Proposition: Don't push generic deals. Instead, emphasize quality, craftsmanship, and long-term value. For instance, highlight durable, premium home goods or investment-grade jewelry.

b. Experiential: Drive them to the mall for non-retail reasons. Offer exclusive access to high-end dining, movie premieres, or specialized services (e.g., tailor, spa).

c. Incentivize First Purchase: Offer a high-quality gift or significant discount tied to a minimum high-value purchase to break their cautious spending habit at the mall.

5. Violet cluster:

a. De-Prioritize: Minimize direct marketing spend on this group.

b. Focus on Necessity: If marketed to at all, focus on extreme discounts, liquidation sales, or basic necessity services (e.g., pharmacy, supermarket if applicable) to capture their occasional, minimal spend.

c. Reactivation: If their spending score was once higher, focus on reactivation campaigns (e.g., "We miss you!") rather than constant, high-cost acquisition efforts.
