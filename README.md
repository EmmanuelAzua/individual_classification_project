Bottom Line - Up Front
1. The Method
* Once I prepareed the dataset, I decided to take a 10k foot view of how the variables interacted with one another
    * I leveraged a correlation heatmap, in which:
        * I decided to make the center of the 1 through -1 range white
        * The darker the color red, the farther away from neutrality each variable was
        * The darker the red color is, the stronger the correlation between two variables is, regardless of the direction of that relationship
2. The Variables
* Thanks to the information the heatmap revealed, I chose the following variable relationships based on correlation strength, and their relationship with the variables "churn" and "tenure". The variable "tenure" is peripherally indicative of customer loyalty to the brand.
For "churn"
1. fiber_optic (0.31)
2. e_check (0.29)
3. tenure (-0.34)
For "tenure"
1. total_charges (0.83)
2. partner (0.39)
3. online_backup (0.39)
4. device_protection (0.38)
5. tech_support (0.34)
6. multiple_lines (0.33)
7. online_security (0.32)
8. streaming_movies (0.3)
9. streaming_tv (0.29)
In the interest of time and efficiency, I chose the variable relationships that are paramount to answering our question. Based on intensity and their impact on churn, the relationships I focused on are:
1. churn / fiber_optic
2. churn / e_check
3. churn / tenure
4. tenure / device_protection
5. tenure / partner
6. tenure / online_backup
I disregarded the "tenure / total_charges" because there is really nothing non-intuitive the linear relationship analysis between time and cummulative costs can really reveal.
3. The Observations
Customers have higher tenures and develop longer relationships with the company when the following factors are present:
1. They have a partner
2. They can leverage online backup
3. They receive device protection
In addition, there seems to be a relationship between longer tenures when customers:
4. Can access tech support
5. Have muplitple lines
6. Can count on online security
7. Leverage the streaming movies service
8. Can stream TV
The opposite is true for customers that:
1. Pay via eCheck
2. Have access to the fiber optic technology
4. The Conclusion
Customers that have a variety of services and add their partners with those services seem to have develop higher levels of brand loyalty.
5. The Recommendation
Develop attractive "family" and group plans that lower the cost of signing up for additional services when signinf more than one person. This will increase customers loyalty, and reduce the rate at which customers churn.
6. The Model
The Decision Tree is the best model to work with this problem definition, in which it operated in a multivariate environment under minimal supervision, based on the following metrics:
Baseline: 0.734
Models' Accuracy with sample data: 0.792
Models' Accuracy without sample data: 0.8


FIRST: I laid out the overall strategy by identifying key moments in the project
1. Global objectives, Requirements, Deliverables, and method

SECOND: I executed the strategy
1. Acquired the data, implemented necessary imports, wrapped each step in python functions, and created easy access files such as CSVs
2. I am a very visual person, so at every step I needed to confirm that the process I was implementing was turning the data the way I needed to
3. Then, I prepared the data, by shedding unnecessary information and turning each variable into a format that was easier for my models to read: binary system, integers (I used dummies, replaced values, etc.0, streamlined and standardized the information formats
4. Once I was finished preparing the dataset, I split it into Train, Validate, and Test groups
5. After I confirmed visually that my group were ready, I explored the data from a 10,000 foot view, in order to figure out the general layout of the variables’ relationships by using a heat map. I preferred to use a method in which, regardless of relationship direction, the color intensity increased as the relationship intensified, as you can see
6. I identified the strongest correlations and had to limit my project to the top 6, in the interest of time
7. Then, I visualized each one of the variables
8. Once I felt confident about my variable selection, I tested their relationship to churn and tenure, since tenure has a peripheral relationship to churn: in a nutshell, customers that churn effectively end their relationship with the company, and reduce their tenure. However, these two variables cannot have a causal relationship.
9. I tested and visualized each relationship I chose. I picked different colors for each relationship to differentiate them
10. The final step in the process, before documenting the work and the results was to turn my stuff into utterable models and determine their accuracy.
11. Even though all my models showed a consistent range of accuracy given the variables that I chose: 78 - 80%, I chose the Decision Tree because it s metrics were the most consistently high in a multivariate environment that requires less supervision for future predictions.

FINALLY: I turned my work into the required documents: .py, csv, and README, and summarized my findings and method.

Pending any questions, this concludes my presentation.

