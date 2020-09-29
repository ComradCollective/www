# Comrad

Comrad is a socialist network. It seizes the means of digital production.

## Why another social network?

Is a 'socialist network' possible? Although the internet began with anarchic design principles, it quickly consolidated into the hands of a few of the largest corporations in the world. It has effectively recreated the capitalist mode of production within itself: the means of content production (social media platforms) are privatized while the work of production (posting) remains socially distributed. Exploitation inheres in that relation, whether in the industrial factory or the digital platform, because the value you produce is taken from you, concentrated and privatized.

But a digital network can be redesigned. The technology behind these social media platforms is actually quite simple. We can easily build our own social network, one which is secure, insurveillable, and unmonetizable—one which would give people the security they need to communicate about whatever they want, including protesting against capital and the state.

## Core principles

### Confidential

All of your data are strongly encrypted end-to-end: only you and those you write to can decrypt and read it. To anyone without the right decryption 'key', the data is nonsense.

### Untraceable

All network traffic is routed through Tor, a "deep web" of computers so dense even the FBI can't follow you through it. Comrad's "Operator" or central server is accessible only from Tor. It's impossible to tell who is sending what to whom, or even who is using the app at all.

### Unmonetizable

What's untraceable is also unmonetizable: your data can't be harvested by technology companies and used for advertising algorithms. You're protected from both surveillance capitalism and the surveillance state.

### Democratized

Group accounts or 'collectives', like @portland or @socialists, grow as existing members 'vouch for' new ones, forming webs of trust. In order to join a group, at least one member must vouch for you; this minimum (or 'quorum') may grow as the group grows, or in accordance with a 'constitution' which the group votes upon.

### (Semi-)decentralized

Data is deleted as soon as possible from Comrad. Comrad's "Operator" simply sorts and holds the mail temporarily: as soon as users log in to download their mail, the messages are deleted from the server and network forever.

### Anti-profit

Not just non-profit, we're anti-profit.

### Open-source

Information wants to be communist.

## Social media features

We present a simplified set of social media features drawn from everything that's out there:

#### Profile
  * Curate a profile with photo and posts (e.g. Twitter)
  * Show profile to world (e.g. Twitter)
  * Show profile only to those you trust (e.g. Facebook)
  * Show profile only to your local area (e.g. Nextdoor)

#### Posting
  * Post up to 1 image and/or 1000 characters
  * Post to the entire world (e.g. Twitter) ✔
  * Post to those you trust (e.g. Facebook)
  * Post to your surrounding area by a distance radius (e.g. Nextdoor)
  * Anonymously up-vote or down-vote posts (e.g. Reddit)

#### Organizing
  * Host events and invite others (e.g. Facebook)
  * Host events like protests anonymously (new)
  * Anonymously pin on a map sites of danger, like police (e.g. Waze)

#### Messaging
  * Message securely with encrypted contents (e.g. Signal) ✔
  * Message with untraceable metadata via Tor (new) ✔


## How is this different from ...?

See ["Comparison of alternative social networks" on the wiki](https://github.com/Comrad/Comrad/wiki/Comparison-of-alternative-social-networks) for an attempt at a systematic comparison. (And please help edit, if you can! The data there is a little incomplete and probably a little inaccurate.) But here are some imagined differences.

* **Comrad is not (fully) decentralized.** Who's afraid of a little central planning? In contrast to [Secure Scuttlebutt](https://scuttlebutt.nz/) and [Cabal Chat](https://cabal.chat/), which are 100% decentralized, subsisting only through peer-to-peer connections, Comrad sticks with the old, client/server model. Why?

* **Comrad is anonymous.** Because P2P networks almost always expose your IP address: they privilege decentralization over anonymity -- and, potentially, safety. By contrast, lying hidden within the deep web of Tor, accessible only from this application and its built-in Tor client, Comrad will never reveal who is accessing it and its encrypted information. This is important for comrades organizing protests against the surveillance state, and to protect our social media traffic from being harvested and monetized by surveillance capitalism.

* **Comrad is 100% end-to-end encrypted.** Unlike [Mastodon](https://joinmastodon.org/) or [Diaspora](https://diasporafoundation.org/), direct messages between users and within groups remain encrypted 1:1 end-to-end among users. Posts to the public are encrypted to @Comrades, a special account which automatically re-encrypts its messages back to any key-registered requester of them.

* **Comrad verifies your identity.** Comrad's server, "The Operator", keeps a permanent record of one thing only: every comrad's name and public key, and requires that new comrades choose a unique name. Whenever you send or receive mail, the Operator will make sure that the name and public key on the letter matches what it has on file, verifying the identity of both parties.

* **Comrad is (semi-)ephemeral.** Data, like all natural things, should not last forever. Direct messages auto-delete from the server as soon as they are downloaded. Group messages are sent as direct messages through the "web of trust" of the group membership network. Posts to the world auto-delete in however many days you specify. By contrast, data on both [SSB](https://scuttlebutt.nz/) and [Matrix](https://matrix.org/) is undeletable.

* **Comrad is simple.** No invitation or server is needed on startup, unlike [SSB](https://scuttlebutt.nz/), [Mastodon](https://joinmastodon.org/), [Diaspora](https://diasporafoundation.org/), or [Briar](https://briarproject.org/). It's basically a Twitter clone, but one where you can also post to a universal feed shared by the entire world (@Comrades), so that you can make yourself known, participate in general discussions, find new contacts, and organize new groups.




## Progress

### Animations from mobile/desktop app

As of the 23rd of August.

<img src="comrad/app/assets/comrad-screen-preview-2020-08-23.gif" alt="GIF animation" />

### Animations from terminal app

#### Connecting through Tor

<img src="comrad/app/assets/comrad-terminal-preview--2020-09-20--tor.gif" alt="GIF animation of Tor connection" />

#### Register/Login

<img src="comrad/app/assets/comrad-terminal-preview--2020-09-16--register.gif" height="500" alt="GIF animation of registering new user" />

#### "Meeting" (exchanging public keys)

<img src="comrad/app/assets/comrad-terminal-preview--2020-09-16--meet.gif" alt="GIF animation of meeting process" />

#### Messaging

<img src="comrad/app/assets/comrad-terminal-preview--2020-09-16--msg.gif" alt="GIF animation of messaging" />

### Posting

<img src="comrad/app/assets/comrad-terminal-preview--2020-09-19--posting.gif" alt="GIF animation of posting" />

### Installing

<img src="comrad/app/assets/comrad-terminal-preview--2020-09-20--install1.gif" alt="GIF animation of installing" />


## Usage

### Install

[Open a terminal](https://towardsdatascience.com/a-quick-guide-to-using-command-line-terminal-96815b97b955), and then copy and paste the following line into it:

```
bash <(curl -s comrad.app/run)
```

Then hit enter. [That](https://github.com/Comrad/Comrad/blob/master/script/micro_installer) grabs a shortcut to [this auto-installer script](https://github.com/Comrad/Comrad/blob/master/script/install). It will install Comrad in a virtual Python environment into a folder of your choosing.

### Run

Install as above.

For the terminal client, run:

```
comrad-cli
```

For the mobile/desktop app, run:

```
comrad-app
```

Or to run the server or Operator (for development only):

```
comrad-op
```


## Details

### Frontend

#### Mobile/desktop

The mobile/desktop app is made with [KivyMD](https://github.com/kivymd/KivyMD), a variant of [Kivy](https://kivy.org/), a cross-platform app development framework in Python. Python is an easy and versatile progamming language to learn, which keeps the code accessible to as many people as possible. Code for the app is in [comrad/app](comrad/app).

#### Terminal app

Vanilla Python. Code is in [comrad/cli](comrad/cli).

### Backend

#### API

Plain old object-oriented code in Python. The root entity is a "Keymaker": anyone from @Telephone, to @Operator, to users, to groups, who has a public/private key pair. The database uses a simple file-based key-value store, written in Python ([simplekv](https://github.com/mbr/simplekv)). Code is in [comrad/backend](comrad/backend).

#### Cryptography

We are using [Themis](https://github.com/cossacklabs/themis), a high-level cross-platform cryptography library, for all cryptographic functions, rather than handling any primitives ourselves.

Code is primarily in:

  * [comrad/backend/keymaker.py](comrad/backend/keymaker.py)

  * [comrad/backend/comrades.py](comrad/backend/comrades.py)

  * [comrad/backend/phonelines.py](comrad/backend/phonelines.py)

