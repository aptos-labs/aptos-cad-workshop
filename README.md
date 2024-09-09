# Aptos create-aptos-dapp Workshop

## Introduction

This workshop will guide you through the process of creating a decentralized application (dApp) using the Aptos
platform.

# Set up prerequisites

Overview:

1. Install Node.js
2. Install Python
3. Install Git
4. Set up a GitHub account
5. Clone the repository
6. Run create-aptos-dapp

Choose your operating system below:

- [Set up for macOS](#prerequisites-macos)
- [Set up for Windows](#prerequisites-windows)
- [Set up for Linux](#prerequisites-linux)

## Prerequisites: macOS

### Recommended: Install with Homebrew

- If you are using macOS, we strongly suggest you install Homebrew, a package manager for macOS. You can
  find [instructions to install it here](https://brew.sh/).
- Once that's done open a terminal with `⌘ Cmd + Space`, typing `terminal`, and pressing `Enter`.
- Then, you can simply run the following commands to install Node.js, Python, and Git:

```bash
brew install node
brew install python
brew install git 
```

#### Verify installation

To verify that you have installed Node.js, Python, and Git correctly, you can run the following commands in the same
terminal

```bash  
node --version
python --version
git --version
```

Afterward, you can proceed to setting up a [GitHub account](#set-up-a-github-account).

### Not recommended: Install Manually

#### 1. Install Node.js

To install Node.js, you can download the installer from the [official website](https://nodejs.org/en/download/).

#### 2. Install Python

To install Python, you can download the installer from the [official website](https://www.python.org/downloads/).

#### 3. Install Git

To install Git, you can download the installer from the [official website](https://git-scm.com/downloads).

#### Verify installation

Once that's done, open a terminal with `⌘ Cmd + Space`, typing `terminal`, and pressing `Enter`.

To verify that you have installed Node.js, Python, and Git correctly, you can run the following commands:

```bash
node --version
python --version
git --version
```

Afterward, you can proceed to setting up a [GitHub account](#set-up-a-github-account).

## Prerequisites: Windows

### Recommended: Install with Chocolatey

Using a package manager like [Chocolatey](https://chocolatey.org/), you can install Node.js, Python, and Git.

First, open a PowerShell window by pressing `⊞ Win + R`, typing `powershell`, and pressing `Enter`.

```powershell
choco install nodejs
choco install python
choco install git
```

#### Verify installation

To verify that you have installed Node.js, Python, and Git correctly, you can run the following commands in the same
PowerShell window:

```powershell
node --version
python --version
git --version
```

Afterward, you can proceed to setting up a [GitHub account](#set-up-a-github-account).

### Not recommended: Install Manually

#### 1. Install Node.js

To install Node.js, you can download the installer from the [official website](https://nodejs.org/en/download/).

#### 2. Install Python

To install Python, you can download the installer from the [official website](https://www.python.org/downloads/).

#### 3. Install Git

To install Git, you can download the installer from the [official website](https://git-scm.com/downloads).

#### Verify installation

First, open a PowerShell window by pressing `⊞ Win + R`, typing `powershell`, and pressing `Enter`.

To verify that you have installed Node.js, Python, and Git correctly, you can run the following commands:

```powershell 
node --version
python --version
git --version
```

Afterward, you can proceed to setting up a [GitHub account](#set-up-a-github-account).

## Prerequisites: Linux

### Recommended: Install with package manager

Using your package manager, you can install Node.js, Python, and Git. Here are some examples:

<details>
<summary>Install with <code>apt</code> (Ubuntu, Debian)</summary>
  
```bash
sudo apt install nodejs
sudo apt install python3
sudo apt install git
```

</details>

<details>
<summary>Install with <code>dnf</code> (Fedora)</summary>
  
```bash
sudo dnf install nodejs
sudo dnf install python3
sudo dnf install git
```
</details>

<details>
<summary>Install with <code>pacman</code> (Arch)</summary>
  
```bash
sudo pacman -S nodejs
sudo pacman -S python
sudo pacman -S git
```
</details>

<details>
<summary>Install with <code>zypper</code> (openSUSE)</summary>
  
```bash
sudo zypper install nodejs
sudo zypper install python3
sudo zypper install git
```
</details>

<details>
<summary>Install with <code>yum</code> (CentOS, AmazonLinux)</summary>
  
```bash
sudo yum install nodejs
sudo yum install python3
sudo yum install git
```
</details>

Afterward, you can proceed to setting up a [GitHub account](#set-up-a-github-account).

### Not recommended: Install Manually

### 1. Install Node.js

To install Node.js, you can download the installer from the [official website](https://nodejs.org/en/download/).

### 2. Install Python

To install Python, you can download the installer from the [official website](https://www.python.org/downloads/).

### 3. Install Git

To install Git, you can download the installer from the [official website](https://git-scm.com/downloads).

### Verify installation

To verify that you have installed Node.js, Python, and Git correctly, you can run the following commands:

```bash
node --version
python --version
git --version
```

Afterward, you can proceed to setting up a [GitHub account](#set-up-a-github-account).

## Set up a GitHub account

To get a copy of this repository, you will need to
have [set up a GitHub account](https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github),
so we can set up a git repository for your project. If you already have one, login to it.

Once you have set up a GitHub account, you can proceed to [forking the repository](#fork-the-repository).

## Fork the repository

To get a copy of this repository, you will need to fork it. Visit [this page](https://github.com/aptos-labs/aptos-cad-workshop/fork)

## Clone the repository

To clone the repository, you will need to copy the URL of your forked repository. You can do this by clicking on the
`Code` button on your forked repository and copying the URL.

Then, open a terminal or command prompt as during installation earlier and run the following command:

```bash
git clone https://github.com/<GITHUB_USERNAME>/aptos-cad-workshop
```

Replace `<GITHUB_USERNAME>` with your GitHub username.

## Optional: Install IDE

If you don't have an IDE, we recommend you install Visual Studio Code. You can download
it [here](https://code.visualstudio.com/Download).

## Install Petra wallet

To install
[download the Petra wallet from the Chrome Web Store](https://chromewebstore.google.com/detail/petra-aptos-wallet/ejjladinnckdgjemekebdpeokbikhfci?pli=1).

Then create a new account: https://petra.app/docs/use#create-a-new-account

And switch to the Testnet network: https://petra.app/docs/use#change-wallet-network

# Create the template dApp

Great!  Now that you have all the prerequisites set up, you can create the template dApp.

To run the `create-aptos-dapp` script, you will need to navigate to the repository you just cloned. You can do this by
running the following command:

```bash
cd aptos-cad-workshop
```

Then, you can run the `create-aptos-dapp` script by running the following command:

```bash
npx create-aptos-dapp@latest
```

It will ask you to confirm with `y` on a message like this:

```bash
Need to install the following packages:
create-aptos-dapp@0.0.22
Ok to proceed? (y) 
```

After you confirm, it will ask you to enter the name of your dApp. Let's enter `workshop` and press `Enter`:

```bash
   ###    ########  ########  #######   ######  
  ## ##   ##     ##    ##    ##     ## ##    ## 
 ##   ##  ##     ##    ##    ##     ## ##       
##     ## ########     ##    ##     ##  ######  
######### ##           ##    ##     ##       ## 
##     ## ##           ##    ##     ## ##    ## 
##     ## ##           ##     #######   ######                                                     

Welcome to the create-aptos-dapp wizard 🌐
? Enter a new project name › workshop
```

After this point, we will want to choose the `NFT minting dapp` option, push down arrow key to select it and press
`Enter`:

```bash
? Choose how to start › - Use arrow-keys. Return to submit.
    Boilerplate Template
❯   NFT minting dapp - A production ready template to create an NFT collection minting dapp
    Token minting dapp
    Token staking dapp
```

Once that is chosen, it will ask you choose your network. Choose `Testnet` by pushing the down arrow key and press
`Enter`:

```bash
? Choose your network › - You can change this later
    Mainnet
❯   Testnet
```

It will then ask you if you want to provide collection anonymous data, choose either `Y` for yes or `N` for no and press
`Enter`:

```bash
? Help us improve create-aptos-dapp by collection anonymous data › (Y/n)
```

Finally, it'll ask you if you want to make any changes, simply press `Enter`:

```bash
? Do you want to make any changes to your selections? (Default is No) › (y/N)
```

Great! You have now created your dApp. You can now navigate to the `workshop` directory by running the following
command:

```bash
cd workshop
```

Let's save our status and push it to our GitHub repository so we don't lose our progress:

```bash
git add .
git commit -m "Initial workshop setup"
git push
```

## Start the dApp locally

You can start the dApp locally by running the following command:

```bash
npm run dev
```

And it will be available to access at http://localhost:5173

# Configure the dApp

This is a simplified version of the dev docs for the NFT Minting
tutorial [here](https://aptos.dev/en/build/create-aptos-dapp/templates/nft-minting-dapp#create-collection-assets)

## Set up the Aptos account

For the dApp to be useful, we will want to create an account and publish an NFT minting contract. First we will
initialize the Aptos account by running the following command and pushing `Enter` through all prompts:

```bash
npm run move:init
```

This will create an account for the dApp to use with an output like:

```bash
npm run move:init

> boilerplate-template@0.0.0 move:init
> node ./scripts/init

Previously installed CLI version 4.0.0, checking for updates
CLI is up to date
Configuring for profile workshop-testnet
Configuring for network Testnet
Enter your private key as a hex literal (0x...) [Current: None | No input: Generate new key (or keep one if present)]

No key given, generating key...
Account 0x7ea046db202cbe947dd5e0e8fe411cbfb14c5bd5c09b10e1ce43c80ec3395866 doesn't exist, creating it and funding it with 100000000 Octas
Account 0x7ea046db202cbe947dd5e0e8fe411cbfb14c5bd5c09b10e1ce43c80ec3395866 funded successfully

---
Aptos CLI is now set up for account 0x7ea046db202cbe947dd5e0e8fe411cbfb14c5bd5c09b10e1ce43c80ec3395866 as profile workshop-testnet!
 See the account here: https://explorer.aptoslabs.com/account/0x7ea046db202cbe947dd5e0e8fe411cbfb14c5bd5c09b10e1ce43c80ec3395866?network=testnet
 Run `aptos --help` for more information about commands
{
  "Result": "Success"
}
```

In this example `0x7ea046db202cbe947dd5e0e8fe411cbfb14c5bd5c09b10e1ce43c80ec3395866` is the account that was created in
testnet. We will now need to put it into the `.env` file in the root of the project. You can do this by editing the
`.env` file or running the following command:

On macOS or Linux, you can run the following command filling in `<address>` with the address from the output above:

```bash
echo "\nVITE_MODULE_ADDRESS=<address>\n" >> .env
```

On Windows, you can run the following command:

```powershell
ECHO "\nVITE_MODULE_ADDRESS=<address>\n" >> .env
```

## Publish the NFT minting contract

Now, we will want to publish our NFT minting contract, so it can be used by the dApp. You can do this by running the
following command and pushing `y` and `Enter` through all prompts:

```bash
npm run move:publish
```

The output will look like:

```bash

> boilerplate-template@0.0.0 move:publish
> node ./scripts/move/publish

Previously installed CLI version 4.0.0, checking for updates
CLI is up to date
Compiling, may take a little while to download git dependencies...
UPDATING GIT DEPENDENCY https://github.com/aptos-labs/aptos-core.git
INCLUDING DEPENDENCY AptosFramework
INCLUDING DEPENDENCY AptosStdlib
INCLUDING DEPENDENCY MoveStdlib
BUILDING MessageBoard
Do you want to publish this package at object address 0x19232670ed920fda00b2e33baa210db21b4d5d9fc68eadf82c03000138eeecc1 [yes/no] >
y
package size 2210 bytes
Do you want to submit a transaction for a range of [327100 - 490600] Octas at a gas unit price of 100 Octas? [yes/no] >
y
Transaction submitted: https://explorer.aptoslabs.com/txn/0xd1b2cee9f8c40aa05afb3b220bbd99533f3c6add56c28af84b251a6d055ef21a?network=testnet
Code was successfully deployed to object address 0x19232670ed920fda00b2e33baa210db21b4d5d9fc68eadf82c03000138eeecc1.
{
  "Result": "Success"
}
```

## Publish the collection

You will need to copy your address from the Petra wallet, if it is not already set up.

On macOS or Linux, you can run the following command filling in `<address>` with the address from your Petra wallet
above:

```bash
echo "\nVITE_COLLECTION_CREATOR_ADDRESS=<address>\n" >> .env
```

On Windows, you can run the following command:

```powershell
ECHO "\nVITE_COLLECTION_CREATOR_ADDRESS=<address>\n" >> .env
```

Now, we will want to publish our NFT collection, this can be done by the UI. Start the website with:

```bash
npm run dev
```

- Navigate to http://localhost:5173.
- Click on the `Connect a Wallet` button. To connect your wallet.
- Click on `Connect` next to `Petra`, to connect your `Petra wallet`.
- Approve the connection in the `Petra wallet` popup.
- Click on the `Create Collection` button. This will publish the collection
- Click `Choose Folder to Upload` and choose the `assets` folder in the root of the project.
- Add now to the public mint start date
- Click `Create Collection` and approve the prompts.

You will then get a collection address, and will need to set `frontend/config.ts`, and fill in the `collection_id`

## Mint NFTs

Going back to the website http://localhost:5173, then you can click the mint button and mint your first NFT!

## Push the dApp to vercel

Now that the collection is published, we will want to publish the dApp to a real website. But first, let's push our
changes to the repository:

```bash
git add .       # Add all files
git add .env -f # Force add the .env file so the website works correctly in Vercel
git commit -m "Added collection details"
git push
```

### Publish via CLI

At this point, you can deploy to Vercel either by running a CLI command if you have a Vercel account:

```bash
npm run deploy
```

It will output something like:

```bash

> nft-minting-dapp-template@0.0.0 deploy
> vercel

(node:3905) [DEP0040] DeprecationWarning: The `punycode` module is deprecated. Please use a userland alternative instead.
(Use `node --trace-deprecation ...` to show where the warning was created)
(node:3905) [DEP0060] DeprecationWarning: The `util._extend` API is deprecated. Please use Object.assign() instead.
Vercel CLI 35.2.4
? Set up and deploy “/opt/git/aptos-cad-workshop/workshop”? yes
? Which scope do you want to deploy to? Greg's projects
? Link to existing project? no
? What’s your project’s name? workshop
? In which directory is your code located? ./
Local settings detected in vercel.json:
Auto-detected Project Settings (Vite):
- Build Command: vite build
- Development Command: vite --port $PORT
- Install Command: `yarn install`, `pnpm install`, `npm install`, or `bun install`
- Output Directory: dist
? Want to modify these settings? no
🔗  Linked to gregs-projects-aeab810b/workshop (created .vercel and added it to .gitignore)
🔍  Inspect: https://vercel.com/gregs-projects-aeab810b/workshop/Hp8f7BjujSVqzf2Li8BKuvRSrdpH [1s]
✅  Production: https://workshop-7xnwd407n-gregs-projects-aeab810b.vercel.app [1s]
📝  Deployed to production. Run `vercel --prod` to overwrite later (https://vercel.link/2F).
💡  To change the domain or build command, go to https://vercel.com/gregs-projects-aeab810b/workshop/settings
```

You can now visit the website at the `Production` link.

You wil need to configure the environment variables in the Vercel project settings. You can do this by visiting the
Vercel website.

### Publish via Vercel website

- You can visit https://vercel.com/login and sign in with your GitHub account, then click on `Add New...` and select
  `Project`.
- Then import the git repository from your account for `aptos-cad-workshop`.
- You will need to configure the `root directory` to `workshop` and the `output directory` to `dist`.
- You may need to copy the environment variables from the `.env` file to the Vercel project settings.

### Expanding upon the workshop

- You can add different stages for mints
- You can build custom flows and animations when people mint NFTs
