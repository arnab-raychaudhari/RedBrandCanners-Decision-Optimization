# RedBrandCanners-Decision-Optimization
Optimization under Quality and Demand Constraints: A Linear Programming Framework for Red Brand Canners’ Production Planning

# Red Brand Canners : Their business
Red Brand Canners is a medium-size company specialising in canning and distributing a variety of
fruit and vegetable products under private brand names in the western states of the US. On Monday,
September 13th, Mitchell Gordon, Vice-President of Operations, asked the Controller, the Sales
Manager, and the Production Manager of Red Brand Canners to meet with him to discuss the amount
of tomato products to pack that season. The tomato crop, which had been purchased at planting, was
beginning to arrive at the cannery. Packing operations would have to start by the following Monday
because, after this time, the fruit would begin to deteriorate. In effect this ruled out the possibility of
reselling any part of the crop which, if it remained unpacked, would be worthless.

William Cooper, Controller, and Charles Myers, Sales Manager, were the first to arrive in Mr.
Gordon's office. Dan Tucker, Production Manager, came in a few minutes later and said that he had
picked up Produce Inspection's latest estimate of the quality of the incoming tomatoes. According to
the report, about 20% of the 3,000,000 pound crop was Grade “A” and the remaining portion Grade
“B”.

Mr. Gordon asked Mr. Myers about the demand for tomato products for the coming year. Mr. Myers
replied that they could sell all of the whole canned tomatoes they could produce. The expected
demand for tomato juice and tomato paste, however, was limited. The Sales Manager then passed
around the latest demand forecast (Exhibit 1) reminding the group that selling prices had been set in
light of long-term marketing strategy of the company, and that potential sales had been forecast at
these prices.

After looking at Mr. Myers’ estimates of demand, Mr. Cooper said that it looked as though the
company, "should do quite well on the tomato crop this year". With the new accounting system that
had been set up, he had been able to compute the contribution for each product, and according to his
analysis the incremental profit on whole tomatoes was greater than for any other tomato product. In
May, after Red Brand had signed contracts agreeing to purchase the grower's production at an average
delivered price of 18 cents per pound, Mr. Cooper had computed the tomato products' contributions
(Exhibit 2).

<b>Exhibit 1. Demand Forecasts</b>

<img src="https://github.com/arnab-raychaudhari/RedBrandCanners-Decision-Optimization/blob/eafc07af093c90a8ecdbaae7fdf5732859b0679c/Auxiliary/Exhibit%201.%20Demand%20Forecasts.png" width="800" />

<b>Exhibit 2. Product Item Profitability (per case)</b>

<img src="https://github.com/arnab-raychaudhari/RedBrandCanners-Decision-Optimization/blob/eafc07af093c90a8ecdbaae7fdf5732859b0679c/Auxiliary/Exhibit%202.%20Product%20Item%20Profitability%20(per%20case).png" width="800" />

Mr. Tucker called Mr. Cooper's attention to the fact that, although production capacity was ample, it
was impossible to produce all whole tomatoes because too small a portion of the crop was “A”
quality. Red Brand used a numerical scale to record the quality of both raw produce and prepared
products. This scale ran from zero to ten, the higher number representing better quality. “A” tomatoes
averaged nine points per pound and “B” tomatoes five points per pound. Mr. Tucker noted that the
minimum average input quality for canned whole tomatoes was eight and for juice six points per
pound. <i>(This meant, for example, that for every pound of “B” tomatoes used in a batch of tomato juice, one-third
pound of “A” tomatoes would have to be used to maintain an average quality level of six points per pound for
the batch.)</i> Paste could be made entirely from “B” grade tomatoes. This meant that whole tomato
production was limited to 800,000 pounds.

Mr. Gordon stated that this was not a real limitation. Recently solicited to purchase 80,000 pounds of
Grade “A” tomatoes at 25½ cents per pound, he had turned down the offer. He thought, however, that
the tomatoes were still available.

Mr. Myers, who had been doing some calculations, said that although he agreed that the Company
"should do quite well this year", it would not be by canning whole tomatoes. It seemed to him that
tomato costs should be allocated on the basis of quality and quantity rather than by quantity only, as
Mr. Cooper had done. Therefore, he had recomputed the marginal profit on this basis and from his
results (see Exhibit 3), believed that Red Brand should use 2,000,000 pounds of the “B” tomatoes for
paste, and the remaining 400,000 pounds of “B” tomatoes and all of the “A” tomatoes for juice. If
demand expectations were realised, a profit contribution of $145,600 would be made in this year's
tomato crop.

<b>Exhibit 3. Myers’ Analysis of Tomato Costs</b>

<img src="https://github.com/arnab-raychaudhari/RedBrandCanners-Decision-Optimization/blob/eafc07af093c90a8ecdbaae7fdf5732859b0679c/Auxiliary/Exhibit%203.%20Myers%E2%80%99%20Analysis%20of%20Tomato%20Costs.png" width="800" />

<b>Exhibit 4. Myers’ Marginal Profit Analysis of Tomato Products</b>

<img src="https://github.com/arnab-raychaudhari/RedBrandCanners-Decision-Optimization/blob/97b98a8d084ce71e1428ddcb293af262bdbcf67a/Auxiliary/Exhibit%204.%20Myers%E2%80%99%20Marginal%20Profit%20Analysis%20of%20Tomato%20Products.png" width="800" />

## The interesting conundrum and how Linear Programming can rescue Red Brand Canners

Locate the sections respective to the following bullets in <a href="https://github.com/arnab-raychaudhari/RedBrandCanners-Decision-Optimization/blob/59c29e1a9a467afdba6685807478c94a4c74456d/RBC-Linear-Programming-Notebook.ipynb" target="_blank">Interative Python Notebook</a> (.ipynb), where I have illustrated the solution for RBC's business problem.

1. <b>Model</b>:

Built a model for the problem RBC is faced with, disregarding the availability of the
additional A tomatoes. Made recommendation about the products to produce along with the required quantities.

<h4>Solution:</h4>

<img src="https://github.com/arnab-raychaudhari/RedBrandCanners-Decision-Optimization/blob/5757899ef83f26c7e33fa917e0842ead72ba2d21/Auxiliary/Part%201%20Solution%20-%20Image%201.png" width="800" />

<img src="https://github.com/arnab-raychaudhari/RedBrandCanners-Decision-Optimization/blob/5757899ef83f26c7e33fa917e0842ead72ba2d21/Auxiliary/Part%201%20Solution%20-%20Image%202.png" width="800" />

<img src="https://github.com/arnab-raychaudhari/RedBrandCanners-Decision-Optimization/blob/5757899ef83f26c7e33fa917e0842ead72ba2d21/Auxiliary/Part%201%20Solution%20-%20Image%203.png" width="800" />

<img src="https://github.com/arnab-raychaudhari/RedBrandCanners-Decision-Optimization/blob/5757899ef83f26c7e33fa917e0842ead72ba2d21/Auxiliary/Part%201%20Solution%20-%20Image%204.png" width="800" />

2. <b>Additional supply of A tomatoes</b> :

Modified the model to incorporate the option of buying the additional 80,000 pounds of A tomatoes at
25.5 cents/pound as suggested by Mitchell Gordon. Answered the following questions.

• Should Gordon buy the additional A tomatoes?

• If yes, how should he allocate the additional A tomatoes to the different products?

• Is there only one optimal allocation?

• Suppose the additional A tomatoes cost more than 25.5 cents/pound. Up to what price should Gordon be willing to pay?

<h4>Solution:</h4>

<img src="https://github.com/arnab-raychaudhari/RedBrandCanners-Decision-Optimization/blob/5757899ef83f26c7e33fa917e0842ead72ba2d21/Auxiliary/Part%202%20Solution%20-%20Image%201.png" width="800" />

<img src="https://github.com/arnab-raychaudhari/RedBrandCanners-Decision-Optimization/blob/5757899ef83f26c7e33fa917e0842ead72ba2d21/Auxiliary/Part%202%20Solution%20-%20Image%202.png" width="800" />

<img src="https://github.com/arnab-raychaudhari/RedBrandCanners-Decision-Optimization/blob/5757899ef83f26c7e33fa917e0842ead72ba2d21/Auxiliary/Part%202%20Solution%20-%20Image%203.png" width="800" />

<img src="https://github.com/arnab-raychaudhari/RedBrandCanners-Decision-Optimization/blob/5757899ef83f26c7e33fa917e0842ead72ba2d21/Auxiliary/Part%202%20Solution%20-%20Image%204.png" width="800" />

<img src="https://github.com/arnab-raychaudhari/RedBrandCanners-Decision-Optimization/blob/5757899ef83f26c7e33fa917e0842ead72ba2d21/Auxiliary/Part%202%20Solution%20-%20Image%205.png" width="800" />

3. <b>Advertising</b>

Suppose that the marketing department of Red Brand Canners feels that it could increase the demand for any of the three tomato products by 5,000 cases, by means of advertising.

• How much should RBC be willing to pay for such a campaign?
• At which product(s) should the advertising be directed?
• Demonstrated how the Sensitivity Analysis report can be used for making this decision.

<h4>Solution:</h4>

Through marketing campaigns, there is a potential to increase the demand for certain product categories, which can lead to increased profitability. If RBC considers creating a surplus demand of 5000 cases, they should focus on Tomato Paste. The Sensitivity Analysis report shows that the Demand constraint for Tomato Paste has a Slack of 0, indicating that it is a binding constraint. Therefore, any additional demand up to <b>2173.33 pounds</b> could still result in surplus profit. However, for the other two product categories, increasing demand may not result in additional profit, as they have a non-zero slack (<b>13580</b> for whole tomato demand and <b>740</b> for tomato juice).

We revised the demand constraint for Tomato Paste from <b>2000</b> to <b>2125</b> (calculated as <b>25 lb/case * (80,000 + 5000)</b>), scaling the number by dividing it by <b>1000</b> as done in previous LP models, and executed a new LP model. As expected, we observed a profit increase of <b>$6041 (=$683,388 – $677,347)</b>. This change in profit can be validated by multiplying the shadow price of <b>48.33 by 125 (2125 – 2000)</b>.

4. <b>Additional supply for B tomatoes</b>

Mitchell Gordon receives a call from Ed Dawkins, the Vice President of Operations at Tomaco, a
company in the same business as Red Brand Canners, active in the Midwest. Dawkins tells Gordon
that they are stuck with some B tomatoes that they cannot put to good use. Dawkins offers Gordon
some of these tomatoes at 18 cents per pound, generally agreed as the “normal” tomato price. Mitchell
Gordon refuses to buy the tomatoes, claiming that the 18 cents per pound is based on the fact that the
incoming crop normally contains a mix of grade A and grade B tomatoes.

• Explained Michell Gordon's reasoning
• Is it worth buying additional B tomatoes at 18 cents per pound?

<h4>Solution:</h4>

RBC has already procured <b>2,400,000 pounds</b> of grade B tomatoes at <b>18 cents per pound</b>. Any additional purchase of grade B tomatoes would only be a sensible decision if it helps in increasing profit. Upon reviewing the Sensitivity Analysis report, we noticed that the Slack against the Supply coefficient of <b>2400</b> is <b>0</b>, proving that we have a binding constraint. Any further increase in supply up to the upper range of <b>3018.33 pounds</b> may result in an increase in profitability. A unit increase in grade B tomato supply can provide us with an additional <b>$173.67</b> worth of profit. To validate this hypothesis, we changed the supply constraint B coefficient from <b>2400 to 2401</b> and executed a new model. As expected, the optimal objective changed from <b>$683,388 to $683,562</b>, representing an increase of approximately <b>$173</b>.

5. <b>Closing down production lines</b>

Starting up the production line for each of the products entails a substantial set-up cost. Dan Tucker
estimates that the set-up costs are $50,000 per line. This means that if RBC decides not to start up a
particular line, they would save $50,000, but they would not be able to produce that particular
product.

• If RBC decides not to start up the Paste line, will this increase or decrease our total profit?
• Which production lines are ideal for RBC to start up?

<h4>Solution:</h4>

Starting up the production line for each product incurs a significant set-up cost, which plays a pivotal role in production planning and budgeting by directly influencing the feasibility and profitability of manufacturing. When considering the termination of a product category, it is essential to incorporate the cost savings into the objective function. This approach allows for a thorough evaluation of profitability and aids in making informed decisions regarding which product line to close, aiming to maximize profits for RBC management.

To assess the impact of terminating specific product lines, we incorporated the estimated savings of $50,000 into our objective function, scaling it appropriately (i.e., <b>50</b>), and implemented a Linear Program using Gurobipy. Our analysis included three scenarios: a) terminating the production of whole tomatoes, b) terminating the production of tomato juice, and c) terminating the production of tomato paste. Upon evaluating these scenarios, we observed a decrease in the objective function to <b>$642,050, $641,383, and $313,161</b>, respectively. It is noteworthy that the decision not to start up the Tomato Paste line significantly diminishes the profit, almost cutting it by more than <b>50%</b>.

Based on these results, RBC would be most profitable by ceasing the production of whole tomatoes, as this decision would still yield a profit of <b>$642,050</b>, the highest among the three scenarios. Hence, they should be most profitable if they start up the production line of Tomato Juice and Tomato Paste. This analysis demonstrates the importance of strategic decision-making in production planning to maximize profitability and operational efficiency.

6. <b>RBC's tomato purchase strategy 1 year later</b>

In April the year after, Red Brand Canners is preparing for the annual negotiations with the tomato
farmers. Although the quality of the crop varies from year to year, the price and quantity are
negotiated in advance. At a meeting, Dan Tucker, William Cooper, Charles Myers and Mitchell
Gordon agree that this year, an acceptable price would be 20 cents per pound, and they are debating how many pounds of tomatoes to contract for. Dan Tucker says that initial discussions revealed that
they could order up to 13 million pounds of tomatoes. Charles Myers says that demand is pretty
much the same as last year, i.e. they would be able to sell as many whole canned tomatoes as they
can make, and demand for juice and paste is again limited to 50,000 and 80,000 cases, respectively.
Also prices and production costs are stable and would be the same as last year. The only
uncertainty is the quality of the crop. Looking at historical data, Tucker observes that in the past
there were basically three types of years. In “wet” years, like last year, the crop was quite poor, and
contained only about 20% grade A. In “sunny” years, the percentage of A tomatoes was around 60%,
and in “normal” years, the crop contained approximately 50% grade A tomatoes. Tucker also
observed that about 25% of the years were “sunny”, 50% “normal” years and 25% “poor”.

• Assuming the forecast of next year to be a sunny year is known in advance, how many pounds of tomatoes
would should RBC buy? Call this <b>(S)</b>. How about for a normal <b>(N)</b> and poor <b>(P)</b> year?
Note that RBC can order at most 13 million pounds.

• Suppose a decision is made to order <b>(S)</b> pounds of tomatoes. What would be the possible outcomes, given that
the year could be sunny, normal or poor? Perform a scenario analysis. Do the same for ordering <b>(N)</b> and <b>(P)</b> tomatoes.

• Given the probabilities of sunny, poor and normal years, what is the average total profit of ordering <b>(S)</b>, <b>(P)</b> and <b>(N)</b> tomatoes?

• What is the recommended amount (pounds) of tomatoes for RBC to buy?

<h4>Solution:</h4>

Over the next year, a decision on the optimal quantity of tomatoes to purchase under different weather conditions needs to be made. The weather forecast suggests there is a <b>25%</b> chance of a sunny year, a <b>50%</b> probability of a normal year, and a <b>25%</b> likelihood of a poor year. Based on these probabilities and the respective profits associated with each scenario, a calculated strategy is imperative for RBC’s success.

We have revised the profit objective formula as it does include the purchasing price:

$$
47 * (a_{w} + b_{w}) - 2 * (a_{j} + b_{j}) + 22 * (a_{p} + b_{p})
$$ 

For a sunny year, RBC should consider purchasing <b>12,000,000 pounds</b> of tomatoes, which is anticipated to yield a profit of <b>$514,000,000</b>. If the year turns out to be normal, the advised purchase is <b>10,667,000 pounds</b>, with an expected profit of <b>$451,333,000</b>. In the event of a poor year, a more conservative purchase of <b>5,467,000 pounds</b> is recommended, which would result in a profit of <b>$206,933,000</b>.
 
The distribution of tomatoes into different product lines is critical for maximizing profits. For instance, in a sunny year, RBC would allocate <b>7,800,000 pounds</b> for whole tomatoes and <b>2,200,000 pounds</b> for grade B tomatoes in the same category, with no tomatoes used for juice. Tomato paste production would utilize <b>2,000,000 pounds</b> of grade B tomatoes, which aligns with RBC’s quality and demand constraints.

To derive the average profit considering the probabilities, we consider the profit contributions from each scenario and weigh them accordingly. This results in an expected average profit, of <b>$382,407,750</b> based on each probability.
 
Assuming RBC prepares for a sunny year, they would purchase <b>12,000,000 pounds</b> of tomatoes. If the year turns out to be sunny indeed, the profit contribution would be <b>$467,000,000</b>. However, if the year is unexpectedly normal, the profit decreases to <b>$420,000,000</b> and for a poor year, it further reduces to <b>$194,400,000</b>.
 
On the other hand, planning for a normal year by purchasing <b>10,667,000 pounds</b> of tomatoes would result in profits of <b>$404,349,000</b> if sunny, <b>$378,233,000</b> if normal, and <b>$177,693,000</b> if poor. This approach offers a moderate profit in sunny conditions but provides more stability and less risk in the event of a poor year.
 
Lastly, if RBC anticipates a poor year and orders 5,467,000 pounds, the profit contributions are the lowest across, with <b>$159,949,000</b> for both sunny and normal years and <b>$112,520,000</b> for a poor year. 
 
Now by taking in mind the probability of each condition and including that into the quality of supplied tomatoes, we get a result of profit contribution of <b>$410,600,000</b> taking into account the probabilities of each weather condition and the quality of supplied tomatoes. This figure seems to be an adjusted profit considering these factors. Bringing the optimal order of <b>9,800,000</b> tomatoes.
