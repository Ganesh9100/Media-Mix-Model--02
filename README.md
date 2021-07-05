# Media-Mix-Modeling-




<p align="center">
  
  <img src="https://github.com/Ganesh9100/Media-Mix-Model--02/blob/main/MMM.png" width="600" height = "800" title="hover text">
  
</p>


# media variables 
<b>online</b>
(display ads, websites, blogging, social media, e-mail
marketing and pay-per-click advertising (PPC)) or/and
<b>offline</b>
(television, radio, newspaper print collateral) – and

# control variables,

seasonality, weather (precipitation and temperature), gross domestic product
(GDP), inflation and market competition information that
accounts for the external factors affecting sales



# Carry-over-effect :
Carryover effects, often called lagged effects,
For example-1 , if we spend $100 on display advertising today, we may not see the effects of this spend for several days.

Example - 2 :  if we spend in TV add for 1 month to sell Hamam Soap then this ad will be able to carryover for some N months so that after that N months we will have to updated the add to make the carryover.

By analyzing this carry over effect, marketers get to know about the purchase frequency and spending pattern of the customers

<b>The adstock function attempts to parameterize this phenomenon</b>

adstock is the cumulative value of a brand’s advertising at a given point in time
<br>
<b>Customer retention rate</b> 
It is the percentage of initial customers who continue to purchase the same product of a particular brand. More the number of repeated visits by the customer; more is the rate of retention.

<b>Customer decay rate:</b>
It is the percentage of initial customers who don’t turn up for repurchase. If less number of customers repurchases the products, the marketer is incapable of holding the consumer to the brand

<b>carryover effect also have another meaning</b> :: It is the difference between customer retention rate and customer decay rate 


# Diminishing Returns

This arises when a media channel starts to loose its effectiveness. 
Example : if a farmer tends to grow crops and he see's that adding much fertilizer will help in much more yeild. 
He started from 1 unit of fertilizer then followed by 2 , 3 ,4 he gets much more return and when he add one more unit of fertilizer ( 5 ) the yeild is low because too much fertilizer will be poisonous 

In out case :: After a certain saturation point, increasing spend will yield diminishing marginal return, the channel will be losing efficiency as you keep overspending on it.

<b>The hill function function attempts to parameterize this phenomenon</b>




















<p>
  # 2.1 Control Model / Base Sales Model
  
<b>Goal: predict base sales (X_ctrl) as an input variable to MMM, this represents the baseline sales trend without any marketing activities.</b>
  

  <b>X1:</b> control variables positively related to sales, including macro economy, store count, markdown, holiday.
  
  <b>X2:</b> control variables that may have either positive or negtive impact on sales: seasonality.
  
  <b>Target variable:</b> ln(sales).
  
The variables are centralized by mean.

# 2.2 Marketing Mix Model
  <b>Goal:</b>
- Find appropriate adstock parameters for media channels;
- Decompose sales to media channels’ contribution (and non-marketing contribution).

L: length of media impact
P: peak of media impact
D: decay of media impact
X: adstocked media impression variables and base sales
  <b>Target variable:</b> ln(sales)
Variables are centralized by means
  
  
  
  
  
  2.3 Diminishing Return Model
  <b>Goal:</b> for each channel, find the relationship (fit a Hill function) between spending and contribution, so that ROAS and marginal ROAS can be calculated.

x: adstocked media channel spending
K: half-saturation point
S: shape
  <b>Target variable:</b> the media channel’s contribution
Variables are centralized by means.
# Reference Blog - Thanks to the author Sibyl He


https://towardsdatascience.com/python-stan-implementation-of-multiplicative-marketing-mix-model-with-deep-dive-into-adstock-a7320865b334
