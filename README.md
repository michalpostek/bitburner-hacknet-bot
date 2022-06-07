<h1>Hacknet Bot</h1>

<p>Farming bot for <a href="https://store.steampowered.com/app/1812820/Bitburner/">Bitburner</a> game.</p>
<p>You can check this guide on <a href="https://steamcommunity.com/sharedfiles/filedetails/?id=2719939448">Steam</a>.</p>

<h2>How it Works</h2>

<p>Bot takes the following steps</p>
<ol>
  <li>Checks cost and <i>production growth</i> of all the possible upgrades</li>
  <li>Calculates <i>profitable ratio</i> of each upgrade</li>
  <li>Sorts elements by ratio descending</li>
  <li>Chooses the first element</li>
  <li>Checks if you can purchase upgrade now, if not, it waits to collect money</li>
  <li>Checks if you can buy new node in less than 30 seconds (you can customize this time), if so, it buys it</li>
</ol>

<p><i>Profitable ratio</i> = Production growth / upgrade cost</p>
<p><i>Production growth</i> = Production after upgrade - current production</p>

<h2>How to use</h2>

<p>Take the following steps.</p>
<ol>
  <li>Run the terminal</li>
  <li>Type <code>nano hacknet-bot.js</code></li>
  <li>Copy the code from main.js file and paste into file you just created</li>
  <li>Save the file</li>
  <li>Back to the terminal</li>
  <li>Type <code>run hacknet-bot.js</code></li>
</ol>

<p>You can customize the time of waiting for purchase node (by default 30s) by passing an additional script argument</p>
<code>
  run hacknet-bot.js 120
</code>
