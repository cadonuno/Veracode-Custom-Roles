# Veracode Custom Roles

Allows for the bulk creation of Custom Roles in Veracode

## Setup

Clone this repository:

    git clone https://github.com/cadonuno/veracode-custom-roles

Install dependencies:

    cd veracode-custom-roles
    pip install -r requirements.txt

(Optional) Save Veracode API credentials in `~/.veracode/credentials`

    [default]
    veracode_api_key_id = <YOUR_API_KEY_ID>
    veracode_api_key_secret = <YOUR_API_KEY_SECRET>

## Run

If you have saved credentials as above you can run:

    python create-custom-roles.py  -f <excel file with the role definitions>.xlsx

Otherwise you will need to set environment variables:

    export VERACODE_API_KEY_ID=<YOUR_API_KEY_ID>
    export VERACODE_API_KEY_SECRET=<YOUR_API_KEY_SECRET>
    python create-custom-roles.py -f <excel file with the role definitions>.xlsx
