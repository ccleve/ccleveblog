+++
author = "Chris Cleveland"
title = "A Clever Theft of Information"
date = "2021-02-25"
draft = true
+++

THIS IS WRONG. Must double check and make sure that I'm not connected.

I'm a believer in online banks. The brick and mortar bank down the street charges excessive fees and provides no services that are of value to me. I've use Schwab Bank online for years for my personal accounts and it works great.

Finding a good online business bank has been hard, though. 

A few years ago I discovered [Azlo](https://www.azlo.com), and it turned out to be terrific. Good software, no fees, responsive staff. Unfortunately, after some big bank gobbled some other big bank which gobbled Azlo, [the banking overlords shut it down](https://www.azlo.com/blog/go-forth-and-azlo). 

So I looked at other options and found [Brex](https://www.brex.com/). Brex ticks all the boxes. Good website, seems focused on adding lots of features, no fees, very high-techy. So I signed up and sent them $5,000 to get started.

In the beginning, it looked fine. I started using the built-in Brex Mastercard to pay for some subscriptions. But when I connected the Brex account to Quickbooks Online, there was a weird glitch. All of the credit card transactions downloaded into Quickbooks were labeled as "Brex Card", with no supporting detail. How was I to know what each transaction was for?

This was odd, because I had been using Quickbooks for many years, and I had never had this problem with any other bank. I've had accounts at Chase, Fifth Third, Wintrust, Schwab, and Azlo. Always, the transaction detail came through without a problem. If older, legacy banks could handle this, why couldn't fancy, bank-of-the-future Brex do it?

So I wrote to customer support. Chat wasn't working, so I sent an email inquiry. Four days later, I got an answer blaming me: apparently I hadn't set things up to "sync expense data".

Ok, fine. I had connected to the Brex account the normal way, through Quickbooks itself, but they wanted me to do it a different way. I went to the Brex site and saw the Brex Quickbooks integration, which was supposed to help me categorize my transactions. I clicked it and got an OAuth screen from Quickbooks to allow Brex to access my Quickbooks account. Not thinking, I signed in.

Quickbooks popped up a message:

>By selecting Connect, you allow Brex to view and update your QuickBooks Online data, as explained below.

>Intuit and Brex may share the information in your Intuit and Brex accounts. Your relationship to Brex and its use of your information are subject to Brex’s Terms of Service and Privacy Policy. To learn more about how Intuit uses your data, see our Privacy Statement.
Disconnect Brex anytime from your MyApps page.

They want access to my internal accounting system? They need to see every transaction I make? Transactions to every vendor, every employee, how much I pay myself, everything?

What. The. Hell.

I write back to Brex: 

>No, I'm not interested in having Brex categorize my transactions. What I have now with other banks in QBO works fine.

>What I need is for the transaction detail to show up in the Description field, instead of just "Brex Card"

Kristin of Brex support wrote back:

>Hi Chris,

>This is Kristin from Brex Support, stepping in for Rachel.

>Apologies for the miscommunication in our previous email. Unfortunately, there is not a way to modify where the transaction details would show up on the Description field. A workaround would be to enable to your expense data, where it would export the transactions' receipts and memos. 

>I'll be happy to attach a guide for reference: https://support.brex.com/how-can-i-export-receipts-and-memos-to-quickbooks-online/

>Please let us know if we may assist further. Thank for you contacting Brex Support - have a wonderful evening. 

>Kindly,
>Kristin

Really, Kristin? You will withhold transaction details from me, making it nearly impossible to do my books, unless I give you full access to my company's internal accounting system?

And Kristin, you say "there is not a way to modify where transaction details show up"? You know that's a lie, right? Yes, Kristin, there is a way, but you *choose not to give it to me*.

*  *  *

And there it is. That's how the theft happens. And now I have to change banks, once again.

Banks rely on the fact that it's really hard to switch. There's a lot of paperwork. When you put your banking information on your invoices, and your customers enter that info into their system so they can pay you via ACH, and you've got to call all of them and tell them to use a different routing/account number, it's a giant hassle.
<p style="text-align: center;">Centered text</p>


    *    *    *

Brex issued a Mastercard to me, and their little trick to get access to my company's internals is a clear violation of the Mastercard rules.

First, Mastercard has ["Transaction Identification Requirements" (Appendix C)](https://www.mastercard.us/content/dam/mccom/global/documents/transaction-processing-rules.pdf) for vendors who accept Mastercard, and says that vendors must give cardholders certain information. These requirements are meaningless if Brex refuses to pass the information through.

Second, [Mastercard specifies the file format of the transaction data](http://smartdatasupport.mastercard.com/CDF3Overview.pdf):

>There are a limited number of required fields in CDF3. This is not a justification for sending just those required fields. Any file comprising just the required data elements will be of almost no use to our mutual customers. Not every field on every record must be populated, but every field for which data can be obtained by the issuer/processor must be populated. (Page 11)

Third, and most important, [Mastercard has explicit rules for its "customers", i.e. banks](https://www.mastercard.us/content/dam/mccom/global/documents/mastercard-rules.pdf). Here's the biggie:

>Provide valid, accurate, complete, unaltered, and consistent data in all authorization and clearing Transaction messages (Section 3.3, page 69).

If anyone reading this blog post knows anyone at Mastercard, please have them look into this. I expect that it wouldn't take long for Mastercard to yank Brex out of the system right quick.
