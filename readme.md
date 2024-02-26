# Setting Up Solana Test Validator Node on Windows

This guide provides step-by-step instructions for setting up a Solana test validator node on a Windows system and checking the balance using the Solana CLI.

## Prerequisites

Before you begin, ensure you have the following installed:
- [Solana CLI](https://docs.solana.com/cli/install-solana-cli/installation)
- Windows system

## Steps

1. **Open Command Prompt with Administrator Privileges**
   - Press `Win + X` on your keyboard.
   - Select "Command Prompt (Admin)" from the menu that appears.

2. **Run Solana Test Validator**
   - In the Command Prompt window, run the following command:
     ```
     solana-test-validator
     ```
   - This command will start a local Solana test validator node.

3. **Get Solana Configuration**
   - After the validator node is running, you can get the current Solana configuration by running:
     ```
     solana config get
     ```

4. **Set Local Network Address**
   - Use the following command to set the local network address (replace `127.0.0.1:8899` with your desired local network address if necessary):
     ```
     solana config set --url http://127.0.0.1:8899
     ```

5. **Check Balance**
   - To check the balance of an account, you need the account's public key. If you have an account public key, you can run the following command to check its balance:
     ```
     solana balance <public_key>
     ```
   Replace `<public_key>` with the actual public key of the account you want to check the balance for.

## Additional Information

- For more information on Solana CLI commands and usage, refer to the [Solana CLI Documentation](https://docs.solana.com/cli/using-the-cli).

## Troubleshooting

- If you encounter any issues during setup, please refer to the official [Solana Documentation](https://docs.solana.com/) or community resources for assistance.
