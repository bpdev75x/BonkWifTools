
![github_banner2](https://github.com/user-attachments/assets/dfc87609-0b93-4ebb-941b-96d11bf12616)


# Bonkwiftools Bundler

Bonkwiftools Bundler is a powerful tool designed to simplify and automate multi-wallet bundle buying on the Solana blockchain, specifically tailored for use with bonk.fun. This innovative solution enables volume generation, sale execution, and bundle validation across 20 wallets simultaneously, delivering high efficiency for advanced users managing fast-paced trading activity.

## Initial Setup

To utilize the Bonkwiftools Bundler effectively, please adhere to the following setup and execution guidelines.

### Step 1: Configuration

- **Edit the `.env` File:** Before executing the script, configure the `.env` file with the required keypairs:

  - **SOL Distribution Fees Keypair:** This keypair handles the payment of all SOL distribution fees.
  - **Pool Creation Keypair:** This keypair facilitates pool creation. For security, these keypairs should be distinct.

  While testing the script, you can use the same keypair for both roles. Always store these keypairs securely.

### Step 2: Execution of Functions

**Note:** To maintain error-free execution, perform these next steps in the correct order.

- **Create Keypairs (Step 1):** While not mandatory for every launch, it's recommended to generate new keypairs initially or during resets to ensure no residual SOL remains in the wallets.

- **Premarket (Step 2):** This multi-step process must be executed in sequence:

  1. **Execution Sequence:** Complete steps 2 through 6 sequentially.
  2. **Bundle ID Validation:** Confirm the Bundle ID after each step to ensure successful landing.
  3. **Repeat if Necessary:** If the bundle fails to land, increase the tip amount and retry.
  4. **Cross-Verification:** Use the Jito Block Explorer to verify landing. Ignore "Landed - no" status and ensure the first transaction is confirmed.

- **Create Pool (Step 3):** Pool creation may require several attempts:

  - Use function spamming if initial attempts fail.
  - Raise the tip to 0.1 SOL or more for better chances of success.

- **Selling Options (Steps 4 and 5):**

  1. **Simultaneous Keypair Sale (Step 4):** Sell from all keypairs at once and reclaim WSOL in Step 7 of Premarket after rugging.
  2. **Percentage-Based Selling (Step 5):** Sell custom percentages by sending partial balances from each keypair to the fee payer before bundling.

- **Liquidity Pool Removal (Step 6):**

  - **Non-Burn Removal:** LP will be removed automatically without the need for a burn.

## Features

- **Launch Modes:** Safe, experimental, timed drop, delay, and volume generator.
- **Sell Modes:** Multiple strategies to match market behavior.
- **Volume Tasks:** Includes micro volume, bumping, human mode, whale trap, chart farming, and more.
- **Comment Bot:** Adds fake engagement to Pump.fun threads.
- **Telegram Auto-Shiller:** Automatically sends token info and messages to multiple Telegram groups.

## Pricing

- **Token Holders:** Hold 10,000,000 $BWT for 7+ days to access the tool for 5 SOL (lifetime).
- **Non-Holders:** Lifetime access available for 10 SOL.

## Tips and Troubleshooting

- **Bundle Success:** If the bundle fails, increase the tip or retry. Use Jito Block Explorer for verification.
- **Keypair Security:** Ensure the keypairs are valid and securely configured in the `.env` file.
- **Spamming Caution:** Be mindful of unnecessary SOL loss during function spamming.

### Final Thoughts

Bonkwiftools Bundler provides a robust solution for managing Solana bundle transactions efficiently across multiple wallets. By following this setup and leveraging its features, you can enhance your performance on bonk.fun and similar platforms.

For technical support, reach out via Telegram: @bonkwiftools
