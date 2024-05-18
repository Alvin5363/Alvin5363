struct SignatureWrapper {
    uint8 ownerIndex;
    bytes signatureData;
}import { StakingClient } from "@coinbase/staking-client-library-ts";

// Set your api key name and private key here. Get your keys from here: https://portal.cdp.coinbase.com/access/api
const apiKeyName: string = 'your-api-key-name';
const apiPrivateKey: string = 'your-api-private-key';

const client = new StakingClient(apiKeyName, apiPrivateKey);

// Note: The below amount is in WEI
const workflow = client.Ethereum.stake('holesky', 'put your wallet address here', '100')
  .then( (workflow) => {
    console.log(JSON.stringify(workflow, null, 2));
  })
  .catch(() => {
    throw new Error('Error running stake action on ethereum');
  });

// Congratulations! You can now sign this unsigned TX & submit it onchain.
// Here is where you would use (ex. https://docs.cdp.coinbase.com/wallet-sdk)
// to have your user sign & submit the staking transaction with their connected wallet.- 👋 Hi, I’m @Alvin5363
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Alvin5363/Alvin5363 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
