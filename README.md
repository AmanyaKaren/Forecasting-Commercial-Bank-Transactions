<h1 style="text-align:center; font-family: 'Times New Roman',Times, serif; font-weight: bold;">Forecasting-Commercial-Bank-Transactions</h1>

Time series analysis and modelling of a commercial bank's transactions
![Bank_Transactions](Images/bank-img.jpg)

Authors: Nobert Akwir, Karen Amanya, Eugene Kuloba, David Mwiti, Anthony Nene

<h1 style="text-align:left; font-family: 'Times New Roman',Times, serif; font-weight: bold;">Overview</h1>
The general objective is to develop a model that will successfully forecast cash transactions that will help NCBA Bank maintain a sufficient cash at its specifc branches.

<h1 style="text-align:left; font-family: 'Times New Roman',Times, serif; font-weight: bold;">Research Questions</h1>
1) Is there predictability in the net cash transactions?

2) During which periods should the bank expect high cash outflows and when should they expect high cash inflows or a combination of both?

3) What is the a common occurence in the closing cash balances (many lows or many highs)?

<h1 style="text-align:left; font-family: 'Times New Roman',Times, serif; font-weight: bold;">Success Criteria</h1>
The following metrics will be used to determine the project's success:

1) Ability of our analysis to provide the bank with actionable insights on the nature of their cash transactions that they can use for better planning cost cutting measures and security needs identification.

2) The final model's accuracy in forecasting future cash balances.

<h1 style="text-align:left; font-family: 'Times New Roman',Times, serif; font-weight: bold;">Data</h1>

The data used in this project is from data world. The data consists of demo bank transaction details(debits and credits) carried out by different customers and includes other details such as the amount, the mode of transaction(either cash, RTGS, EFT, SWIFT e.t.c), the account's balance at the time of the transation, the time of the transaction e.t.c

<h1 style="text-align:left; font-family: 'Times New Roman',Times, serif; font-weight: bold;">Modelling</h1>
Two models were used ;

1) ARIMA

2) SARIMA

<h1 style="text-align:left; font-family: 'Times New Roman',Times, serif; font-weight: bold;">Evaluation</h1>

<ol>
    <li>ARIMA model - the model overfitted on the train and performed poory on the test data.</li><br>
    <li>SARIMA model -  the model perfromed fairly well on both the train and test data. It captured the monthly seasonaity in the cash balalnces well but did not capture the extreme values.</li><br>
    <li>Further attempts to reduce the variance and seasonality present in the data failed. The sarima model perfromed worse on the data after the second differencing.</li><br>

</ol>


<h1 style="text-align:left; font-family: 'Times New Roman',Times, serif; font-weight: bold;">Conclusion</h1>
   Findings

<ol type='square'>
    <li >There is seasonality in cash transactions - we observed spikes in cash withdrawals at the end of the year and 
in the mid -year around June.A high volume of cash credits is also observed in the mid and end of year periods(June and December)</li><br>
    <li> There are more instances where the cash withdrawals outweighed the cash balances -
indicating that the bank frequently requested for extra cash to cover heavy withdrawals.</li><br>
    <li>There was no observed correlation between a particular day of the week and the net cash balance.</li><br>
    <li>There is predictability in the cash balances - our final model was able to capture correctly the monthly seasonality in the cash balances. The model however, did not capture instances where there were extreme values.</li><br>
</ol>








