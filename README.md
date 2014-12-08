BlockMarket
===========
BlockMarket creates a realistic market system that emulates that of a stock market, allowing players to buy/sell blocks to each other. Once players place items in the vault located in their bank, they can buy/sell those blocks on the open market. Items purchased will be placed in the player's vault, and the money for items sold will be deposited into their account. The player does not have to be online in order for transactions to take place, but will be notified of any transactions that occured while they were offline at login.

Current Version
---------------
Version 1.0.7

Dependencies
------------
Requires the BlockBank and Vault plugins.

Authors
-------
Drewper & Hitechwizard, those great guys running Drewpercraft.com! Come see the plugin in action at minecraft.drewpercraft.com

Commands:
=========
Requirements:

Buying Blocks - In order to place a buy order, your account must have enough money to make the purchase. Your order will only be visible in the market if your vault has enough space available to accept the order.

Selling Blocks - The items to be sold should already be placed in the vault before attempting to sell them. While they are on the market, they will be placed in a holding account until your sell order is executed or cancelled. When the blocks are sold, your bank account will be credited for the sale of the items, less commissions.

Cancelling orders

Buy orders are cancelled immediately and the money refunded to your account.

Sell orders are cancelled only if there is room in the vault they were taken from to put them back.

Player Commands:
================
/market list {buy|sell} {block name} - Show all the buy/sell orders in the market

/market cancel {block name} - Cancel all orders to buy or sell.

/market help - Show the commands available

/market info - Show the open and closing times for the market

/market list {buy|sell} {blockname} - Show what items are currently on the market. Filters are optional

/market price {block name} - Display the lowest current sell price available that would be filled along with the historical average, low and high prices seen in the market.

/market register - Registers the player as a BlockTrader

/buy [block name] {quantity} {price} - Attempt to buy blocks from the market at the given price or less.

/sell [block name] {quantity} {price} - Attempt to sell blocks from the market at the stated price.

/worth - Shows the market price information of the block currently in your hand.

Admin Commands:
===============
All of these commands will apply to the current world. Only one market per world is allowed.

/market create {name} - Creates the market with the given name

/market update open [hour] - Set the Minecraft hour that the market opens

/market update close [hour] - Set the Minecraft hour that the market closes

/market update name {market name} - Changes the displayed named of the market.

/market update commission [percentage] - Set the bank's commission for processing the transaction

Aliases
=======
/market

/bm

Permissions
===========
blockmarket.admin - Can update the market system

blockmarket.buy - Player is allowed to place buy orders

blockmarket.sell - Player is allowed to place sell orders