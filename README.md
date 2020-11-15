# AI-Credit-Risk-Management-for-Social-Lending
Project for designing AI solution for Credit Risk Appraisal in Social Lending

Final project for the Building AI course

## Summary

Social loans are loans provided to individuals who are unable to get reasonable terms of credit elsewhere, but who are nevertheless able to repay loans. To my knowledge credit risk is not appraised with a risk model in any of 30+ Finnish municipalities.

## Background

Most municipalities base their lending decision on payment allowance, which is a calculated as of difference of necessary costs (food, apartement) and sources of income. Payment allowance is maximum amount for loan paybacks and interest. According Terveyden ja hyvinvoinnin laitos (1) total capital for new sosial loans in 2019 was 3,6 million euros, out of which Helsinki amounted half. What is interesting is that there is no information on amount of capital outstanding nor number of total lenders. Social lending or lending in general is not core function for municipalities. It is not surprising that credit risk assessment is some what incoherent. 

Social lending is by nature high risk lending as customers are cut off all other sources of funding due financial distress or other reasons. Traditional credit risk assessment models are not suitable. Decision to approve or disapprove social loan is in my experience based mostly on payment allowance. Model quantifies risk associated with other factors like term of unemployment and common behaviour patterns associated with loan default. It should be stressed that model is not approve or disapprove model. It is more of risk category model, if risk categories are from least risk A to D then ceteris paribus customers same payment allowance but A risk category could have loan up to maximum payment allowance. Granting loan is admunistrative ruling made by social security worker. Model will make rulings more transparent both to customers and social security professionals.  

## How is it used?

Municipalities have quite similar processes for applying and granting social loans. City of Helsinki process (2) is good description of regular process. Their application form for social loan is also a good source for model data. Social Lending is like walking on right rope. Social security worker has to judge whether customer is unable or unwilling to serve social loan. If loan is not granted customer may end up insolvent.

## Data sources and AI methods
All data is sensitive customer data and thus restricted only to persons directly involved with customer. Quality of data varies, one of the reasons is how data systems are set-up. Social security services do not have in my opinion tradition of data management from service production point of view. Data is managed and collected to fulfill legal and administrative obligations. Data is sensitive information on income, employment, debts, assets etc. It has to be anonymized and gathering will probably require invidual research application to every municipality asked for data. AI net has to predict willingness to pay (model past credit behaviour) and ability to pay (model possible shocks to income, costs, and assets). Model training requires data for loan defaults, which might be unsystematically collected to information systems. There are at least 4 or 5 major information systems in use for social services at municipal level. All data collected is provided as-is, data collected and data format will most likely be variable. Considering the challanges in data content, sensitivity (=complete anonymization required) and current culture conserning data usage of social services, all data gathering is done in the project.

## Challenges

This tool will not decide whether loan is granted or not. To some extent social services are trapped to notion that all customers are individuals. This is true but no customer is a beign never seen before. There are factors predicting or forecasting certain behaviour or risks of behaviour. Biggest risk for this project is that model is seen as approval machine. 

## What next?

Preliminary data gathering. I am unfamiliar with short-term loans credit risk models, some insight to these would be welcome. After data or sufficient large samalle is ready, some statistical classification is required to keep number of variables reasonable (at least until my skills with Python or Java are improved).

## Sources
1) https://thl.fi/fi/tilastot-ja-data/tilastot-aiheittain/sosiaalipalvelut/tilastokysely-kuntiin/sosiaalinen-luototus#:~:text=Sosiaalinen%20luototus%202019%20%2D%20Kuntakyselyn%20osaraportti,-Tilastoraportti%20liitteineen&text=Suunnitteilla%20sosiaalinen%20luototus%20oli%209,yhteens%C3%A4%203%2C6%20miljoonaa%20euroa.
2) https://www.hel.fi/sote/fi/palvelut/palvelukuvaus?id=2937
