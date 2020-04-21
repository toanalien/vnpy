# By Traders, For Traders.

<p align="center">
  <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
</p>

<p align="center">
    <img src ="https://img.shields.io/badge/version-2.1.2-blueviolet.svg"/>
    <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
    <img src ="https://img.shields.io/badge/python-3.7-blue.svg" />
    <img src ="https://img.shields.io/github/workflow/status/vnpy/vnpy/Python%20application/master"/>
    <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
</p>

vn.py it is based on a set of Python quantitative trading system open source development framework ， to 2015 year 1 officially released ， in the open source community 6 years of continuous contribution to the growth of quantitative trading platform next step is a full-featured ， currently financial institutions, domestic and foreign users has exceeded 500 home ， include ： private equity 、 securities dealers and information management 、 futures and information management subsidiary 、 university research institutions 、 proprietary trading company 、 exchange 、Token Fund wait 。

 new 《vn.py advanced full combat 》 series of online courses ， it has been the official micro-channel public number [**vnpy-community**] online ， cover CTA tactics （ completed ）、 options volatility trading （ updating ） and so on 。 after purchase, please scan the next fanger wei code concerns ， click on the menu bar 【 advanced courses 】 button ：

<p align="center">
  <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy_qr.jpg"/>
</p>

 in use vn.py secondary development （ tactics 、 modules, etc. ） have any questions about the process ， please check [**vn.py project documentation **](https://www.vnpy.com/docs/cn/index.html)， if you can not solve the go [** official community forum **](https://www.vnpy.com/forum/) of 【 question for help 】 plate for help ， also welcomed 【 experience sharing 】 share your experience using plate ！

 against vn.py users of financial institutions ， we created a special 【vn.py institutional users group 】（QQ group number ：676499931）， the main application sharing mechanism related issues ， such as ： inter-bank market access 、 information management O32 system 、 distributed content deployment 。 please note that this group is only available to users of financial institutions ， plus group please specify ： full name - mechanism - department 。

##  features 

1.  full-featured quantitative trading platform （vnpy.trader）， integrates multiple transaction interface ， and it provides a simple and easy to use for a particular strategy algorithm and feature development API， rapid construction required for traders quantitative trading application 。

2.  all transactions covering domestic and foreign varieties of the transaction interface （vnpy.gateway）：

    *  domestic market 

        * CTP（ctp）： domestic futures 、 options 

        * CTP Mini（mini）： domestic futures 、 options 

        * CTP securities （sopt）：ETF options 

        *  pegasus （femas）： domestic futures 

        *  hang seng UFT（uft）： domestic futures 、ETF options 

        *  core width （oes）： domestic securities （A share ）

        *  china and thailand XTP（xtp）： domestic securities （A share ）、ETF options 

        *  hang seng options （hsoption）：ETF options 

        *  华鑫奇 point （tora）： domestic securities （A share ）

        *  flying bat （sgit）： gold TD、 domestic futures 

        *  xin housekeeper （xgj）： futures and information management 

        *  rong hang （rohon）： futures and information management 

        *  meeting in yida （comstar）： inter-bank market 

    *  overseas market 

        *  fu passers securities （futu）： hong kong stocks 、 us stocks 

        *  tiger securities （tiger）： global securities 、 futures 、 options 、 foreign exchange 

        * Interactive Brokers（ib）： global securities 、 futures 、 options 、 foreign exchange 

        *  yi sheng 9.0 external disk （tap）： global futures 

        *  direct futures （da）： global futures 

        * OANDA（oanda）： exchange 、CFD

        * Alpaca（alpaca）： us stocks （ zero commission ）

    *  digital currency 

        * BitMEX（bitmex）： digital currency futures 、 options 、 sustainable contracts 

        * Bybit（bybit）： sustainable digital currency contracts 

        * OKEX sustainable （okexs）： sustainable digital currency contracts 

        * OKEX futures （okexf）： digital currency futures 

        * OKEX options （okexo）： digital currency options 

        *  fire currency contracts （hbdm）： digital currency futures 

        *  an coins sustainable （binancef)： sustainable digital currency contracts 

        * Gate.io sustainable （gateios）： sustainable digital currency contracts 

        * Deribit（deribit）， digital currency options 、 sustainable contracts 

        *  an coins （binance）： digital currency spot 

        * OKEX（okex）： digital currency spot 

        *  fire currency （huobi）： digital currency spot 

        * Bitfinex（bitfinex）： digital currency spot 

        * Coinbase（coinbase）： digital currency spot 

        * Bitstamp（bitstamp）： digital currency spot 

        * 1Token（onetoken）： digital currency broker （ stock 、 futures ）

    *  special applications 

        * RPC service （rpc）： cross-process communication interface ， for distributed architecture 

3.  all kinds of quantitative strategies trading applications out of the box （vnpy.app）：

    * cta_strategy：CTA policy engine module ， while maintaining the ease of use ， to allow for users CTA process class policy to run in the report commissioned by the withdrawal behavior of fine-grained control （ reduce transaction slippage 、 high frequency strategies ）

    * cta_backtester：CTA strategy backtesting module ， without the use of Jupyter Notebook， direct use graphical interface directly strategy backtesting analysis 、 parameter optimization and other related work 

    * spread_trading： spread trading module ， support for custom spreads ， real-time quotes and to calculate the spread positions ， support for semi-automatic and fully automatic algorithmic trading spreads spread trading strategies two modes 

    * option_master： options trading module ， design options for the domestic market ， it supports a variety of option pricing model 、 implied volatility surface computing 、 greece value risk tracking and other functions 

    * portfolio_strategy： combine policy module ， at the same time quantitative strategies for trading contracts and more （Alpha、 options arbitrage, etc. ）， back-tested historical data and automated trading firm functions 

    * algo_trading： algorithmic trading module ， it offers a variety of commonly used smart trading algorithms ：TWAP、Sniper、Iceberg、BestLimit and many more ， support for common algorithm configuration is saved 

    * script_trader： scripts policy module ， for multi-target combination class trading strategy design ， at the same time can also be implemented directly on the command line REPL instruction in the form of transaction ， backtesting feature is not supported 

    * chart_wizard：K line graph module ， based on RQData data service （ futures ） or transaction interface （ digital currency ） obtain historical data ， combined Tick push display real-time market changes 

    * portfolio_manager： portfolio module ， fundamentals for all types of trading strategies ， to separate policy-based subaccounts ， providing trade position of the automatic tracking and real-time profit and loss statistics 

    * rpc_service：RPC service module ， allows a VN Trader process starts for the server ， as a unified market and transaction routing channel ， it allows multiple simultaneous client connections ， multi-process distributed systems 

    * data_manager： historical data management module ， view profile data already in the database through the directory tree ， select any period of time to see the field data details ， stand by CSV data import and export files 

    * data_recorder： quotes recording module ， be configured based graphical interface ， according to the needs of real-time recording Tick or K quotes line into the database ， backtesting for strategy or firm initialization 

    * excel_rtd：Excel RTD（Real Time Data） real time data services ， based on pyxll module implemented in Excel the acquisition of various types of data （ price 、 contract 、 positions, etc. ） real-time push updates 

    * risk_manager： risk management module ， including transaction provides flow control 、 under a single number 、 principal activities 、 statistics and limit the total number of regular withdrawals ， effective to achieve the control function of the front end of the wind 

4. Python transaction API interface package （vnpy.api）， the deal provides an interface to achieve the underlying docking 。

5.  simple and easy to use event-driven engine （vnpy.event）， as the core of event-driven trading programs 。

6.  inter-process communication standard components （vnpy.rpc）， system implementation for complex transactions distributed deployment 。

7. Python high performance K line chart （vnpy.chart）， support large amount of data in the chart display and real-time data updates 。

8. [ community forum ](http://www.vnpy.com) with [ know almost column ](http://zhuanlan.zhihu.com/vn-py)， content include vn.py tutorials and project development Python the contents of applied research in the field of quantitative trading 。

9.  the official exchange group 262656087（QQ）， strict management （ periodically clear long-term member of diving ）， the fee will be donated to the group vn.py community fund 。

##  preparing the environment 

*  recommended use vn.py quantitative trading team built specifically Python release [VNStudio-2.1.2](https://download.vnpy.com/vnstudio-2.1.2.exe)， built with the latest version of the vn.py framework and VN Station quantitative management platform ， no need to manually install 
*  support system version ：Windows 7 the above /Windows Server 2008 the above /Ubuntu 18.04 LTS
*  supported Python version ：Python 3.7 64 place （** note must be Python 3.7 64 bit versions **）

##  installation steps 

 in [ here ](https://github.com/vnpy/vnpy/releases) download the latest version ， after extracting run the following command to install ：

**Windows**

    install.bat

**Ubuntu**

    bash install.sh

##  user's guidance 

1.  in [SimNow](http://www.simnow.com.cn/) registered CTP simulation account ， and [ this page ](http://www.simnow.com.cn/product.action) get the code and brokers trading market server address 。

2.  in [vn.py community forum ](https://www.vnpy.com/forum/) register for VN Station account password （ forum account password that is ）

3.  start up VN Station（ installation VN Studio after automatically create a shortcut on the desktop ）， enter your login account and password on step 

4.  click the bottom **VN Trader Lite** push button ， start your transaction ！！！

 note ：

*  in VN Trader do not turn off the process of running VN Station（ it will automatically exit ）
*  if you need the flexibility to configure quantitative trading application components ， please use **VN Trader Pro**

##  script 

 in addition to on VN Station graphical way outside to start ， you can also create any directory run.py， the following sample code is written ：

```Python
from vnpy.event import EventEngine
from vnpy.trader.engine import MainEngine
from vnpy.trader.ui import MainWindow, create_qapp
from vnpy.gateway.ctp import CtpGateway
from vnpy.app.cta_strategy import CtaStrategyApp
from vnpy.app.cta_backtester import CtaBacktesterApp

def main():
    """Start VN Trader"""
    qapp = create_qapp()

    event_engine = EventEngine()
    main_engine = MainEngine(event_engine)
    
    main_engine.add_gateway(CtpGateway)
    main_engine.add_app(CtaStrategyApp)
    main_engine.add_app(CtaBacktesterApp)

    main_window = MainWindow(main_engine, event_engine)
    main_window.showMaximized()

    qapp.exec()

if __name__ == "__main__":
    main()
```

 open in the directory CMD（ press and hold Shift-> right click -> open a command window here /PowerShell） after you run the following command to start VN Trader：

    python run.py

##  contributing code 

vn.py use Github managed its source code ， if you want to contribute code to use github of PR（Pull Request） process :

1. [ create  Issue](https://github.com/vnpy/vnpy/issues/new) -  for larger changes （ as new features ， large-scale reconstruction, etc. ） a good idea to open issue discuss ， smaller improvement（ such as documentation improvements ，bugfix wait ） sent directly PR to 

2. Fork [vn.py](https://github.com/vnpy/vnpy) -  click on the top right **Fork** push button 

3. Clone your own fork: ```git clone https://github.com/$userid/vnpy.git```
	*  if your fork outdated ， need to manually sync：[ synchronization method ](https://help.github.com/articles/syncing-a-fork/)

4.  from **dev** create your own feature branch: ```git checkout -b $my_feature_branch dev```

5.  in $my_feature_branch on modify and amend push to your fork on 

6.  creating your fork of $my_feature_branch branch to the main project **dev** branch [Pull Request] -  [ here ](https://github.com/vnpy/vnpy/compare?expand=1) click on **compare across forks**， select the desired fork with branch create PR

7.  wait review,  we need to continue to improve ， or is Merge!

 when submitting code ， please observe the following rules ， to improve code quality ：

  *  use [autopep8](https://github.com/hhatto/autopep8) format your code 。 run ```autopep8 --in-place --recursive . ``` to 。
  *  use [flake8](https://pypi.org/project/flake8/) check your code ， ensure that no error with warning。 run in the project root directory ```flake8``` to 。



##  project donation 

 past 6 years received many donations user community ， in this deeply grateful ！ all donated funds are put into the vn.py community fund ， for support vn.py operation of the project 。

 to emphasize ：**vn.py it is an open source project ， it can be permanently free of charge ， and there is no mandatory requirement to donate ！！！**

 donations ： alipay 3216630132@qq.com（* xiao excellent ）

 long-term maintenance of a list of donations ， please indicate in the message is a project donor and the donor's name 。

##  other content 

* [ getting help ](https://github.com/vnpy/vnpy/blob/dev/.github/SUPPORT.md)
* [ community conduct side ](https://github.com/vnpy/vnpy/blob/dev/.github/CODE_OF_CONDUCT.md)
* [Issue template ](https://github.com/vnpy/vnpy/blob/dev/.github/ISSUE_TEMPLATE.md)
* [PR template ](https://github.com/vnpy/vnpy/blob/dev/.github/PULL_REQUEST_TEMPLATE.md)

##  copyright statement 

MIT
