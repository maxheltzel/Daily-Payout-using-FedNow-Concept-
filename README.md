# Daily-Payout-using-FedNow-Concept

This is just a concept, there are a lot of issues, like calculations of payments, taxes, and more...
That's for you to figure out.


Introduction:

	PayNow is a financial application designed to provide consumers with immediate compensation for their work. The system utilizes various technologies and APIs to streamline the payment process and ensure fast and accurate payouts.

To track hours worked, PayNow integrates with third-party APIs such as UKG (Ultimate Kronos Group) to gather precise data on the user's working hours. This API enables real-time synchronization of work hours, ensuring accurate calculations for timely compensation.

Alternatively, PayNow leverages the power of Artificial Intelligence (AI) algorithms to calculate the daily wage payout. By analyzing various factors such as work hours, job type, and pay rates, the AI engine accurately determines the amount that users should be paid for each day's work.

To enable instant payouts, PayNow leverages Real-Time payment rails such as FedNow and the RTP® Network. These payment networks facilitate the immediate transfer of funds, ensuring that users receive their earnings promptly after completing their work.

The combination of seamless API integration, advanced AI algorithms, and real-time payment infrastructure empowers PayNow to provide users with a fast and efficient solution for receiving their wages on a daily basis.


Preface: 

PayNow solves the problem of delayed compensation for individuals after they have completed their work. Traditional payroll systems often have a delay between the time when work is performed and when the payment is processed, which can range from a few days to a few weeks. This delay can create financial stress and inconvenience for workers who rely on their income for day-to-day expenses.

By offering immediate payouts, PayNow addresses this problem by providing individuals with instant access to their earnings. This allows workers to receive their compensation as soon as they complete their work, eliminating the waiting period typically associated with traditional payroll cycles.

PayNow also caters to individuals who may have irregular or gig-based employment where they perform various short-term jobs. Such workers often face challenges in receiving timely and consistent payments. PayNow's ability to track hours worked and calculate daily wage payouts addresses this issue by ensuring that individuals are compensated promptly for their efforts.

Overall, PayNow streamlines the payment process, reduces financial uncertainty, and provides individuals with greater financial control and stability by solving the problem of delayed compensation.






Problem:

	The problem with the current same-day get-paid services is the inability to receive much of the paycheck. Services like DailyPay pay out half of what you earned to mitigate the risk of overages or shorts due to taxes and fees. They also charge an absurd transaction fee of 3$ on every transaction [which can be troublesome for users who earn a low wage].
	All current applications require employer collaboration which isn't very intuitive in the days of APIs and AI.
According to a CNBC, “Your Money Financial Confidence Survey”, conducted in partnership with Momentive, 70% of Americans are feeling financially stressed due to inflation, economic instability, and a lack of savings [1]. Additionally, a report released by LendingClub Corporation and PYMNTS reveals that 60% of consumers in the United States lived paycheck to paycheck as of March 2023 [3]. Furthermore, a survey found that 65% of paycheck-to-paycheck consumers have experienced a financially stressful event in the past three years [2].
	Living paycheck to paycheck can be a major source of stress for Americans, as it can lead to a range of financial difficulties and negative effects. According to a report by the American Psychological Association, financial worries are one of the leading causes of stress among Americans [4]. Some of the snowballing effects of living paycheck to paycheck can include increased debt, missed payments, and reduced savings. This can make it difficult to cover unexpected expenses and can also impact long-term financial goals, such as retirement planning.
Furthermore, a recent survey by the National Endowment for Financial Education found that those living paycheck to paycheck are more likely to experience financial stress, which can lead to a range of physical and mental health problems [5]. In addition, struggling to make ends meet can also impact job performance and lead to increased absenteeism and lower productivity [6].
	
Solution:
	According to a study done by PYMNTS, offering employees the option to receive their pay on a daily basis can help reduce financial stress and improve overall financial wellness [8]. When employees are paid daily, they have better control over their finances and are less likely to rely on high-interest loans or credit cards to cover expenses between paychecks. This can lead to improved credit scores, reduced debt, and increased savings. Additionally, daily pay can help reduce the negative impact of financial stress on physical and mental health, as well as job performance and productivity. Overall, providing employees with daily pay options can be a win-win situation for both the employer and the employee [9].
PAYNOW uses the FedNow wire system which is an interbank real-time gross settlement system (RTGS) that settles payments through an API-based payment message exchange system [10]. The system provides immediate access to funds once a payment message is received, allowing for instant payment services [11]. FedNow settles payments through the participating banks' accounts held at the Federal Reserve, which rely on databases and wire transfer technologies to manage the flow of funds [12]. The system requires banks to develop sophisticated intraday liquidity management and cash flow forecasting capabilities to ensure reliable and efficient transactions [10]. Fraud management is also a key concern, and the system includes fraud-specific items in its readiness checklists [10]. Overall, FedNow's real-time payments system offers a secure and reliable solution for businesses and individuals to send and receive payments instantly, providing flexibility and improving financial wellness.
By using domestic RTP rails, PayNow can use internal APIs which coerce real-time executable payments to give payouts based on reported hours worked or divisible calculations on a reported salary.
	PayNow then collects a direct deposit at the end of the pay period and if there ends up being an overage or shortage, the internal API’s will credit/debit the necessary accounts in which are connected using Plaid[13] (or a preferred open banking system).
	PayNow allows for (and starts with) manual entry, as it is subject to lesser risk.
	
	THE USP for PayNow is the ability to receive 70% of your paycheck

	
Problems with the Solution and the Solution to Said Problems:

If there is an overage or shortage on an early paycheck payment, it can affect the books and technology in several ways.
Firstly, it would impact the accuracy of the payroll records. If an overage occurs, it could lead to an overstatement of wages and salaries, which would impact the company's financial statements. If a shortage occurs, it could lead to an understatement of wages and salaries, which could cause issues with employee morale.
From a technology standpoint, an overage or short could also cause issues with the payroll software. If the software is not designed to handle these types of adjustments, it could cause errors in the calculations.
To mitigate these issues, it's important to have robust payroll software that can handle adjustments and corrections. Additionally, it's important to have proper controls in place to ensure that payroll records are accurate and free from errors. This could include implementing a system of checks and balances, such as having multiple people review the payroll records before processing payments.

Receiving paychecks can sometimes be unverifiable because of elusive scheduling or misuse of systems like [UKGworkforce] to exploit internal APIs.


To receive paychecks, the user must submit their sub-account [ACC NUMBER, etc…] (if using the master-account model) information to their employer as their direct deposit, as well as their desired destination account (which will be connected using open banking [13]. 

The user has to process their entire hourly paycheck through PayNow’s system unless compensated on a salary basis due to the lack of verifiable schedule knowledge and the risk of real-time schedule change faults.

Internal risk detection systems would be able to detect when there is a fault in transponded data due to excessive/ exacerbating hours, which will then have to be verified by the user so no overage is credited.



__________________________________________________
USE CASE - Scenario
Use Case: 
Enabling Daily Paychecks for Employees using FedNow
Overview:
FedNow is a real-time payments system developed by the Federal Reserve that enables instant payment processing 24/7/365. One potential use case for FedNow is to enable daily paychecks for employees, which can help reduce financial stress and improve overall financial wellness. This use case explores how FedNow can be used to facilitate daily paychecks for employees.
Key Stakeholders:
- Employers
- Employees
- Financial institutions
- Federal Reserve
Benefits:
- Reduces financial stress for employees
- Improves overall financial wellness
- Increases employee retention and job satisfaction
- Provides instant access to funds for employees
- Reduces the need for payday loans and other high-interest credit options
Scenario:
1. Employees opt-in to receive daily payments to their bank accounts or digital wallets.
2. When an employee completes their workday, the employer’s hourly “calculator” (i.e. UKGworkforce) sends completed and verified hours through the payroll system that is processed instantly and paid with FedNow or RTP network.
3. The payment is credited to the employee's bank account or digital wallet instantly, providing them with immediate access to funds.
4. Employees can use the funds to pay bills, make purchases, or save for future expenses without having to wait for their next paycheck.
Conclusion:
Providing Americans with an everyday salary/wage payout app can help relieve financial stress and potentially boost the economy. The app would allow employees to access their earned wages before payday, providing them with a financial cushion and reducing the need for payday loans and credit card debt. This, in turn, can decrease financial stress, increase productivity and reduce employee turnover. Here's how this technology can benefit both employees and the economy as a whole.
Firstly, financial stress is a significant problem in the US, with 65% of respondents in a survey by the American Psychological Association stating that money is a significant source of stress [16]. This stress can lead to reduced productivity, absenteeism, and employee turnover, all of which are detrimental to the economy. By providing an everyday salary/wage payout app, employees have access to their earned wages before payday, which can reduce the need for payday loans and credit card debt. This reduces financial stress and can potentially increase productivity and reduce employee turnover [17].
Secondly, providing access to earned wages before payday can help employees manage their finances better. With an everyday salary/wage payout app, employees can budget their expenses more efficiently, pay bills on time, and avoid overdraft fees. This can help employees build an emergency savings fund, which can be beneficial during financial emergencies, such as job loss or medical emergencies. This, in turn, can lead to increased financial stability and potentially increased consumer spending [17].
Thirdly, an everyday salary/wage payout app can potentially boost the economy by increasing consumer spending. With access to earned wages before payday, employees have more disposable income to spend on goods and services, leading to increased consumer spending. This can help boost the economy by creating jobs, increasing tax revenue, and facilitating economic growth [18].
In conclusion, providing Americans with an everyday salary/wage payout app can help relieve financial stress, increase productivity, reduce employee turnover, and potentially boost the economy. This technology can provide employees with a financial cushion, reduce the need for payday loans and credit card debt, and help employees manage their finances better. By increasing consumer spending, an everyday salary/wage payout app can potentially boost the economy by creating jobs, increasing tax revenue, and facilitating economic growth.
___________________________
References:
[1] 70% of Americans feel financially stressed, new ...
[2] 65 Percent of Paycheck-to-Paycheck Consumers ...
[3] At 73%, Millennials Are the Most Likely Generation to Live …
[4] https://www.apa.org/news/press/releases/stress/2019/stress-in-america-money
[5]https://www.nefe.org/Press-Room/News/2020/National-Survey-Reveals-How-Paycheck-to-Paycheck-L.aspx
[6] https://www.shrm.org/resourcesandtools/hr-topics/benefits/pages/financial-stress
[7] 90% of Americans Stress About Money, According to Study ...
[8] Coping with Financial Stress
[9] The Financial Stress of Living Paycheck to Paycheck
[10] FedNow real-time payment (RTP) system
[11] The Fed - Frequently Asked Questions
[12] How do real-time payments work? | PaymentsSource
[13] Plaid is a popular open banking platform that connects fintech apps to customers' financial accounts. It uses APIs to access data from various financial institutions and databases to store and manage the data securely. To mitigate the risk of fraud, Plaid uses advanced security measures such as multi-factor authentication, biometric identification, and transaction monitoring. When a customer authorizes a fintech app to access their financial data, Plaid uses OAuth to generate a token that the app can use to access the data. Plaid also uses encryption and tokenization to ensure that sensitive data is protected. Overall, Plaid's technology enables the safe and secure sharing of financial data, providing consumers and businesses with improved financial transparency and access to innovative financial products and services.
[14] MASTER ACCOUNT ref. - In this model, a fintech startup partners with a single bank that provides a macro bank account to manage all user financial accounts. The fintech startup then creates sub-accounts for each user within the macro account to manage their funds. This model allows fintech startups to offer banking services without obtaining a banking license and enables them to avoid the regulatory hurdles that come with managing individual bank accounts for each user. However, it also poses risks such as concentration risk, where the failure of the master account could affect all sub-accounts.
[15] OMNIBUS ACCOUNT ref. In this model, a single account is used to hold funds on behalf of multiple clients, with each client having their own sub-account within the omnibus account. This model is commonly used in investment management and can help simplify administrative tasks, reduce costs, and streamline operations. However, it also poses some risks, such as the commingling of funds, lack of transparency, and potential conflicts of interest. As with any financial model, it is important to implement proper controls and risk management strategies to mitigate these risks.
[16] American Psychological Association. (n.d.). Stress in America: Paying with our health. Retrieved from https://www.apa.org/news/press/releases/stress/2021/pay-health
[17] Forbes. (2020, July 23). How on-demand pay is relieving financial stress for workers. Retrieved from https://www.forbes.com/sites/forbestechcouncil/2020/07/23/how-on-demand-pay-is-relieving-financial-stress-for-workers/?sh=4b5c7b7a7bf4
[18] Brookings Institution. (2021, April 29). The impact of on-demand pay on the economy. Retrieved from https://www.brookings.edu/blog/up-front/2021/04/29/the-impact-of-on-demand-pay-on-the-economy/
