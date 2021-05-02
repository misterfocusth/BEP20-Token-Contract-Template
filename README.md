# BEP20-Token-Contract-Template
Binance Smart Chain (BEP20) Token Template

A BEP20 token must implement the interface `IBEP20` in [IBEP20.sol](https://docs.binance.org/smart-chain/developer/IBEP20.sol). This is a template contract [BEP20Token.template](https://docs.binance.org/smart-chain/developer/BEP20Token.template). Users just need to fill in `_name`, `_symbol`, `_decimals` and `_totalSupply` according to their own requirements:

    constructor() public {  
	    _name = {{TOKEN_NAME}};  
	    _symbol = {{TOKEN_SYMBOL}};  
	    _decimals = {{DECIMALS}};  
	    _totalSupply = {{TOTAL_SUPPLY}};  
	    _balances[msg.sender] = _totalSupply;  
	    emit Transfer(address(0), msg.sender, _totalSupply); 
	}

Then users can use [Remix IDE](https://remix.ethereum.org/) and [Metamask](https://docs.binance.org/smart-chain/wallet/metamask.html) to compile and deploy the BEP20 contract to BSC.

Credit  : https://docs.binance.org/smart-chain/developer/BEP20.html
