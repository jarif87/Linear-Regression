# Linear-Regression

![This is an image](https://miro.medium.com/max/640/1*LEmBCYAttxS6uI6rEyPLMQ.png)

# What Is Regression?

Regression searches for relationships among variables. For example, you can observe several employees of some company and try to understand how their salaries depend on their features, such as experience, education level, role, city of employment, and so on.

This is a regression problem where data related to each employee represents one observation. The presumption is that the experience, education, role, and city are the independent features, while the salary depends on them.

Similarly, you can try to establish the mathematical dependence of housing prices on area, number of bedrooms, distance to the city center, and so on.

Generally, in regression analysis, you consider some phenomenon of interest and have a number of observations. Each observation has two or more features. Following the assumption that at least one of the features depends on the others, you try to establish a relation among them.

In other words, you need to find a function that maps some features or variables to others sufficiently well.

The dependent features are called the dependent variables, outputs, or responses. The independent features are called the independent variables, inputs, regressors, or predictors.

Regression problems usually have one continuous and unbounded dependent variable. The inputs, however, can be continuous, discrete, or even categorical data such as gender, nationality, or brand.

Itβs a common practice to denote the outputs with π¦ and the inputs with π₯. If there are two or more independent variables, then they can be represented as the vector π± = (π₯β, β¦, π₯α΅£), where π is the number of inputs.


# When Do You Need Regression?

Typically, you need regression to answer whether and how some phenomenon influences the other or how several variables are related. For example, you can use it to determine if and to what extent experience or gender impacts salaries.

Regression is also useful when you want to forecast a response using a new set of predictors. For example, you could try to predict electricity consumption of a household for the next hour given the outdoor temperature, time of day, and number of residents in that household.

Regression is used in many different fields, including economics, computer science, and the social sciences. Its importance rises every day with the availability of large amounts of data and increased awareness of the practical value of data.

# Linear Regression :

Linear regression is probably one of the most important and widely used regression techniques. Itβs among the simplest regression methods. One of its main advantages is the ease of interpreting results.

# Problem Formulation :
When implementing linear regression of some dependent variable π¦ on the set of independent variables π± = (π₯β, β¦, π₯α΅£), where π is the number of predictors, you assume a linear relationship between π¦ and π±: π¦ = π½β + π½βπ₯β + β― + π½α΅£π₯α΅£ + π. This equation is the regression equation. π½β, π½β, β¦, π½α΅£ are the regression coefficients, and π is the random error.

Linear regression calculates the estimators of the regression coefficients or simply the predicted weights, denoted with πβ, πβ, β¦, πα΅£. These estimators define the estimated regression function π(π±) = πβ + πβπ₯β + β― + πα΅£π₯α΅£. This function should capture the dependencies between the inputs and output sufficiently well.

The estimated or predicted response, π(π±α΅’), for each observation π = 1, β¦, π, should be as close as possible to the corresponding actual response π¦α΅’. The differences π¦α΅’ - π(π±α΅’) for all observations π = 1, β¦, π, are called the residuals. Regression is about determining the best predicted weightsβthat is, the weights corresponding to the smallest residuals.

To get the best weights, you usually minimize the sum of squared residuals (SSR) for all observations π = 1, β¦, π: SSR = Ξ£α΅’(π¦α΅’ - π(π±α΅’))Β². This approach is called the method of ordinary least squares.

# Regression Performance
The variation of actual responses π¦α΅’, π = 1, β¦, π, occurs partly due to the dependence on the predictors π±α΅’. However, thereβs also an additional inherent variance of the output.

The coefficient of determination, denoted as πΒ², tells you which amount of variation in π¦ can be explained by the dependence on π±, using the particular regression model. A larger πΒ² indicates a better fit and means that the model can better explain the variation of the output with different inputs.

The value πΒ² = 1 corresponds to SSR = 0. Thatβs the perfect fit, since the values of predicted and actual responses fit completely to each other.
