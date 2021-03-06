# Cypress LL training

### Prerequisite:
* Linux native environment or Windows.
    <pre><code>To setup in WSL please check "Setup WSL" guide in confluence</code></pre>

### Requirements:
1. Node.js
2. yarn
3. git
4. Visual Studio Code: https://code.visualstudio.com/

# WINDOWS
## Node.js:
Donwload and install from: https://nodejs.org/en/download/

## yarn:
Donwload and install from: https://yarnpkg.com/lang/en/docs/install/#windows-stable

## git:
Download and install from: https://git-scm.com/download/win


# LINUX
## Node.js:
We are going to use nvm, which is a version manager for node, makes it easier to mantain the node version.
1) Instal nvm, with: 
<code>curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.2/install.sh | bash</code>
2) To verify installation, enter command<code>nvm --version</code> ...this should return something like<code>'0.33.3'</code>, if you receive <code>'command not found'</code> or no response at all, close your current terminal, reopen it, and try again.
3) Install latest v10 version of Node.js (recommended for NGA): <code>nvm install 10</code>
4) Verify that Node.js is installed and the currently default version with: <code>node --version</code>. Then verify that you have npm as well, with: <code>npm --version</code>

## yarn
1) Add the repository to your installation:
    <pre>
    <code>curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -</code></pre>
    <pre>
    <code>echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list</code></pre>
2) Update and install yarn
<pre><code>sudo apt update && sudo apt install --no-install-recommends yarn</code></pre>

## git
1) Start by updating the package index:
<code>sudo apt update</code>
2) Run the following command to install Git:
<code>sudo apt install git</code>
3) Verify the installation by typing the following command which will print the Git version:
<code>git --version</code>

# Download and use this repo AFTER all of the above is installed
1) Create a 'repos' folder wherever is convinient for you (I recommend having it somwhere like .../Documents/repos)
2) Open a new terminal and navigate to that folder
3) Run the following command: 
    <pre><code>git clone https://github.com/OjelaNape/cypress_training.git</code></pre>
4) Open Visual Studio Code, go to Files -> Open folder -> Search and open "cypress_training" 
6) In your terminal run your corresponding: 
    <pre><code>git checkout marian</code></pre>
    <pre><code>git checkout caro</code></pre>
    <pre><code>git checkout djurdja</code></pre>
    <pre><code>git checkout adrian</code></pre>
> This will get your own branch to keep the code separate, but share one common base to install dependencies and plugins. Now that you have your code in your computer with your own branch to go nuts, lets install all the dependencies.
7) In your terminal run: <code>yarn</code> (Yeah, just that, nothing else)
8) Wait until done
9) In your terminal, run: <code>yarn cypress open</code>
> IF no errors come up, you are golden.
