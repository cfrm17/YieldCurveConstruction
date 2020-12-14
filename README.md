# Yield Curve Construction

Yield curve is defined as the term structure of interest rate yields-to-maturity. Yield curves are not market observable and need to constructed from market observable curves, such as bond curves or swap curves. Given swap market is much more liquid than bond market with narrow bid-ask spreads and a wide selection of maturities, yield curves are mainly bootstrapped from swap curves.

Yield curves belong to derived interest rate curves. You can find more information on interest rate curve category. A yield curve, commonly used to forecast or discount an asset value, is essential in valuation. Yield curve is widely regarded as the best proxy for risk-free curve and benchmark curve.

The shape of yield curve implies future interest rate expectation and economic forecasting. It helps market participants to understand market behavior, trends, and risk. It is also used as a funding curve among different counterparties in financial market. You can find more information about curve data convention, quotation, list, and API.

Zero rate curve or par yield curve or spot rate curve is a special type of yield curve, that is defined as the term structure of the yields-to-maturity of zero coupon bonds. Zero rates and discount factors have a very simple one-to-one relationship as

     D(t,T) = exp (-rT)

where D(t,T) is the discount factor at time t for maturity T and r is the continuously compounded zero rate or spot rate between time t and T.

This relationship makes zero rate curves an essential valuation vehicle in financial market and a dominant type of yield curve. In general, zero rate curves and yield curves are equivalent. When people talk about yield curves, they actually mean zero rate curves.

Zero rate curves also have many different types. A zero curve derived from a 3 month swap curve is usually called 3 month zero rate curve. Similarly, a zero rate curve bootstrapped from a 6 month basis swap curve is called 6 month zero rate curve, and so on and so forth. Each has its specific utilization. Understanding interest rate curves is essential in financial markets.

Prior to the 2007 financial crisis, financial institutions performed valuation and risk management of any interest rate derivatives on a given currency using a single-curve approach. This approach consisted of building a unique curve and using it for both discounting and forecasting cash flows. However, after the financial crisis, basis swap spreads were no longer negligible and the market was characterized by a sort of segmentation. Consequently, market practitioners started to use a new valuation approach referred to as multicurve approach, which is characterized by a unique discounting curve and multiple forecasting curves

The current methodology in capital markets for marking to market securities and derivatives is to estimate and discount future cash flows using rates derived from the appropriate term structure. The yield curve is increasingly used as the foundation for deriving relative term structures and as a benchmark for pricing and hedging.

Yield curves are derived or bootstrapped from observed market instruments that represent the most liquid and dominant interest rate products for certain time horizons. Normally the curve is divided into three parts. The short end of the term structure is determined using LIBOR rates. The middle part of the curve is constructed using Eurodollar futures or forward rate agreements (FRA). The far end is derived using mid swap rates.

The objective of the bootstrap algorithm is to find the zero yield or discount factor for each maturity point and cash flow date sequentially so that all curve instruments can be priced back to the market quotes. All bootstrapping methods build up the term structure from shorter maturities to longer ones.

You can find more details at
https://finpricing.com/lib/IrCurveIntroduction.html
