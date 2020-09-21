# Algorithmic Trading - Price Impact & Order Flow
Implementing a medium freq trading strategy by estimating price impact via order flow.  

The trading strategy starts by retrieving parameters from the running window, it uses the Dickey-Fuller test to see if the centered Orderflow is stationary or not.
If it is, then the price impact factor from order flow can be used to estimate the target prices. We will the proceed to long or short an asset if we expect it to be profitable. 
After we reach one of the stopping conditions (max holdin time, exceeding price boundaries etc.), we close the position by buying or selling back our assets and the change in price should yield us a profit. See pdf and python notebook for more details.
