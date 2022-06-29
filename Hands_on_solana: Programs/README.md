# Solana_Concept_With_Rust
#Programs

Prerequsit:

    [Nodejs](https://nodejs.org/en/download/)
    [I'm an inline-style link](https://www.google.com)
    [GitHub Pages](https://pages.github.com/)
        Command: sh -c "$(curl -sSfL https://release.solana.com/v1.10.29/install)"
        This will take a couple of hours to get the installation complete. You can take a cup of coeffe/chilled stuff or just relax and breath 🧘🏽‍♂️ while the installation is running

This is the introductry aspect of solana with Rust 

    Introductory commands: 

    solana config set --keypair /home/xi6th/.config/solana/id.json
    solana config set --url http://api.devnet.solana.com
    nano /home/xi6th/.config/solana/cli/config.yml
    solana config set --url https://api.devnet.solana.com
    nano /home/xi6th/.config/solana/cli/config.yml
    solana config set --url https://api.devnet.solana.com
    nano /home/xi6th/.config/solana/cli/config.yml
    solana logs
    solana balance
    solana airdop 2

By deafult Linux dosent recognise the path which solana is installed. However you can export to the rigth path with the path generated after the installation.

    command:  export  PATH="/home/xi6th/.local/share/solana/install/active_release/bin:$PATH" 👈🏽👈🏽👈🏽

Generating a keypair is enssential for development and production phase of solana application.
    
    Reason: To have a recognised solana account 🤔🤔🤔
    Command : solana-keygen new 👈🏽👈🏽👈🏽

    Generating a new keypair

    For added security, enter a BIP39 passphrase

    NOTE! This passphrase improves security of the recovery seed phrase NOT the
    keypair file itself, which is stored as insecure plain text

    BIP39 Passphrase (empty for none): 

    Wrote new keypair to /home/xi6th/.config/solana/id.json 👍 👍 👍 
    ============================================================================
    pubkey: 2ci2eXbWxdfsihBGP1bhVYJBCuj7HuCd4inWxykEJ5vF
    ============================================================================
    Save this seed phrase and your BIP39 passphrase to recover your new keypair: 👍 👍 👍 
    waste soon patrol elbow reform resemble quit voice salt large vessel various

From the description above the most important aspect of the output generated are:

    1.  Directory to which your keypairs are saved: /home/xi6th/.config/solana/id.json
    2.  Seed phrase and your BIP39 passphrase: [waste soon patrol elbow reform resemble quit voice salt large vessel various]

    Caution 🚫: Please key output 2 private and never share with anyone. This is expose because of educational purpose 👌🏽👌🏽👌🏽.

After generating keyspairs, you need to configure your solana account
    
    Command: solana config set --keypair <Directory to which your keypairs are saved> 👈🏽👈🏽👈🏽

Next you need to connect to solana network:

    There are couple of network to connect to which are:
        devnet: https://api.devnet.solana.com
        mainnet: https://api.mainnet.solana.com 
        testnet: https://api.testnet.solana.com
    
    However for development purpose it best to connet using the devnet. 
        Reason: You need Sol to pay gas fees and rent fees.  🤔🤔🤔

In order to check the coonfiguration of your connection you can use this linux command:

    command : nano <Directory to which your keypairs are saved> 👈🏽👈🏽👈🏽

Final aspect of the setup is to purchase the Sol:

    command: solana airdop 2 👈🏽👈🏽👈🏽
    Since you're connected to the devnnet environment you wont be charged for the SOL purchase made. You can get as much as you want. I Got 20 SOl for testing 😂😂😂