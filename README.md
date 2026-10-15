# Federal Credit Banking — Simulation

A fictional banking interface for local software practice. It is not affiliated with any real bank or credit union, and it does not connect to payment rails or move real money. Keep the simulation notice visible if you customize the interface.

## Run locally

1. Extract the folder and open it in Visual Studio Code.
2. Open Terminal → New Terminal.
3. Run `npm install`.
4. On the first run, choose a password for the local accounts by setting an environment variable in PowerShell:

   ```powershell
   $env:INITIAL_ACCOUNT_PASSWORD = "ChooseYourOwnStrongPassword123!"
   npm start
   ```

   Choose your own password; do not reuse a real banking password. The server hashes this password for the two fictional accounts when their password hashes are empty. After first initialization, the hashes are saved in `data/accounts.json`, so you do not need to set this variable on every restart.

5. Open `http://localhost:3000`.

## Fictional account usernames

- `jordan.taylor`
- `alex.morgan`

Both accounts use the password you chose during first-time setup. Account numbers are fictional and are only for testing transfers inside this local simulation.

## Notes

- All balances and transactions are fictional and denominated in USD.
- Data is stored locally in `data/accounts.json`.
- This project is not production-ready and must not be used to collect real credentials, account details, deposits, or payments.
- For any public deployment, keep the simulation disclaimer visible and use a proper database, secret management, HTTPS, and a security review.
