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
