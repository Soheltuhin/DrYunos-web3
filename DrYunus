<!DOCTYPE html><html>
<head>
  <title>DrYunos Wallet Checker</title>
  <script src="https://cdn.jsdelivr.net/npm/web3@latest/dist/web3.min.js"></script>
</head>
<body>
  <h2>Check BNB Wallet Balance</h2>
  <input type="text" id="address" placeholder="Enter wallet address" />
  <button onclick="getBalance()">Check Balance</button>
  <p id="balanceResult"></p> <script>
    async function getBalance() {
      const address = document.getElementById("address").value;
      const web3 = new Web3("https://bsc-dataseed.binance.org/"); // BSC Mainnet
      try {
        const balance = await web3.eth.getBalance(address);
        const bnb = web3.utils.fromWei(balance, "ether");
        document.getElementById("balanceResult").innerText = `Balance: ${bnb} BNB`;
      } catch (error) {
        document.getElementById("balanceResult").innerText = `Error: Invalid address or network issue.`;
      }
    }
  </script></body>
</html>
