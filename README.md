# Junk Drawer
Wikipedia: _"A junk drawer is a drawer used for storing small, miscellaneous, occasionally useful objects of little to no (or unclear) monetary value, and possibly significant sentimental value."_

Home for miscellaneous ideas &amp; unfinished projects in their unpolished state; preserved for future inspiration/scavenging 

## Contents

<details>
<summary>
Hedged Equity
</summary>

### [Hedged Equity](/hedged_equity)

- folder holding various stages of development, raw testing, and abandoned functionality
- most up-to-date version lives in repo [here](https://github.com/loganprob/hedged-equity)
- working on writing documentation, explanation of the math/finance used [here](/hedged_equity/documentation.md)

</details>



<details>
<summary>
Risk Playground
</summary>
  
### [Risk Playground](/risk_playground.ipynb)

- the idea was to be able to quantify different aspects of risk tolerance/appetite by having investors interact with risk in a natural, familiar way: a GUI that mimics their brokerage's phone app (as opposed to unnatural, and in my experience, unreliable 'risk questionaires')
- the intended usage would involve the app's appearance exactly matching how a client normally views their portfolios (accounts named properly, up-to-date account values)
- client would be coached by the advisor to be honest and vocal about their level of unease during use
- the GUI would show risk in different interactive ways, appearing as the client's actual account are experiencing the price movement, such as:
  - different levels of daily volatility (up and down)
  - sharp drawdowns of increasing magnitude
  - pairs of positive and negative moves that represent equivalent likelihood movements, to illustrate diminishing utility. E.g.
    - "I am indifferent to experiencing a +2% vs a -2% day, but a -10% day is much more negative to me that a +10% day is positive"  
- advisor would be taking notes, facilitating conversation, and performing the task of translating the intensity of client emotions to predetermined spots on a probability distribution, e.g.
  - -1σ likelihood ≈ "Bad day, don't want to look at my account balances until tomorrow"
  - -2σ likelihood ≈ "I'm likely to call you to ask what's going on in the market"
  - -3σ likelihood ≈ "You'd be fired in this scenario"
- the code would be responsible for translating all of the collected data points into a few key metrics to aide in portfolio construction and conversations about risk
  
![image](https://github.com/loganprob/junk_drawer/assets/56107919/5e6ba77b-db08-48f4-9abe-1a7e456c4642)

- this was a one-day project (and obviously, not very aethetically appealing) to test implementation. I really like the idea, and would like to return to it one day. Maybe just a standalone website

</details>


<details>
<summary>
Bond Simulation
</summary>

### [Bond Simulation](/bond_simulation.ipynb)

- this was a one-off project for a specific portfolio to simulate how it might perform vs some other portfolio under various future yield curve scenarios
- ipython widgets, very ugly, but a fun proof-of-concept to build further functionality upon
- pursuing better performance and user experience, this turned into a javascript [project](https://loganprob.github.io/yieldcurve.html) with much better graphics and controls
- had started building JS functionaly to allow for drag and drop loading different CSV holdings exports from custodians into the tool + manual bond entry, but development slowed down because javascript is awful
- like the "risk playground" project, it would be cool to finish this as a standalone website
- Example of the original jupyter notebook (lots happening!):

![image](https://github.com/loganprob/junk_drawer/assets/56107919/a6526392-872f-4299-b634-e0e2d0500581)

</details>


<details>
<summary>
Google Database/API
</summary>

### [Google Database/API](/google_database_api)

- a huge undertaking... still very much a work-in-progress with not a ton of public progress to show
- this project has already tought me a ton about technical areas of which I had no prior knowledge or experience, like no-SQL database management and asynchronous programming
- more fundamentally, this is really the first project I've worked on that doesn't run solely on my machine with my expected inputs (and my ability to step in and make fixes when things go wrong), meaning lots and lots of thinking about potential problems, error handling, and ["failing eloquently"](https://www.amazon.com/Designing-Data-Intensive-Applications-Reliable-Maintainable/dp/1449373321)
- another related lesson I learned was that, while it is fun, trying to write code as cleverly and concisely as possible is not the end goal. The poor soul (me) that has to continue developing and troubleshooting previously written code (by me) appreciates clarity far more
- also learned the hard way, suprisingly, that SEC filings are the wild-west; every typo (misspelled tickers) and schema invalidation (holdings reports that loop back to themselves) that you can imagine, currently exists in SEC filings. The actual prevelance of errors is probably very low, but when you're trying to write rules for processing tens of thousands of securities, they stick out and break your code
- files in this folder contain miscellaneous (non-linear) building and testing
- there currently exists a live version of the API that (so far) will reliably return basic security information and fund holdings, but given the difficulties outlined above and the fact that my credit card is tied to its usage, I'm going to keep the details under wraps for now
- currently upgrading my desktop's CPU and RAM primarily to iterate local development more rapidly on this project... it's a long-term investment
  
</details>
