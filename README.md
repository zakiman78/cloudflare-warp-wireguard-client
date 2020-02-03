# Cloudflare Warp WireGuard Client
A tool to generate WireGuard profiles from a new or existing Cloudflare Warp account

## Features
- Fetch configuration data from server
- Use existing account
- Create new account
- Check account type / Warp+ status
- Create WireGuard profile

## Usage
- `poetry install`
- `poetry run python wgcf.py`

Your new account details will be saved under `wgcf-identity.json` and your WireGuard profile under `wgcf-profile.conf`

## Existing account
Create a new file `wgcf-identity.json` with your account details in the following format:
```json
{
    "account_id": "",
    "access_token": "",
    "private_key": ""
}
```

## Extracting from Android [ROOT ONLY]
- To obtain the `account_id` and `access_token`, you can:
  - Grab the application's private data and read the shared preferences ([Titanium Backup](https://play.google.com/store/apps/details?id=com.keramidas.TitaniumBackup))
