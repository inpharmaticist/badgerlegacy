# Badger Legacy
A community protocol for inheritance, recovery, and dead man’s switch

## Preamble
Bitcoin inheritance is difficult and we don’t have many examples of successful execution. There are several services available that will set you up and connect with your heirs at the cost of ongoing fees and loss of privacy.

With open-source tools, and the community spirit of the San Diego Bitcoiners, we can model commercial services as a community protocol that has no monetary cost to the user and can improve upon missing aspects like maintenance and accountability.

## Goals
* Create a guideline that can be followed by anyone
* Allow flexibility with details
* Promote self-custody best practices
* Make an execution plan that will ease the burden of mourning loved ones
* Maintain privacy
* Support coordination when requested
* Capitalize on the human connection an in-person meet up group provides
* Build good habits that become rituals

## Problems to Solve
* People have different methods of storing bitcoin and use different tools
* We all have a different tolerance of sharing personal info
* Our loved ones (aka heirs) are often less technical and will likely be distraught if dealing with unexpected death/incapacitation
* You’ll likely never know if your inheritance plan works because you’ll be gone

## Toolbox
* Open source wallets (Sparrow, Blue Wallet, Nunchuk, etc)
* Seed features
  * Descriptor info
  * Passphrase
  * Multisig (and musig2?)
  * Seed XOR
  * Border wallets
* Cryptography – signatures (PGP/Nostr), encryption (PGP, veracrypt, etc), Open Timestamps
* Trusts & Wills
* NDAs
* Waivers

## Criteria
* Partner with at least 2 other people
* Set a maintenance cadence (e.g. every quarter) and deadline (e.g. within a week)
* Share wallet info sufficient for your beneficiary to recover funds, but not enough for inheritance partners to see wallet balance
* Share an optional dead man’s switch and who the message should be sent to
* Establish identity requirements
* Sign NDAs and waivers acknowledging the risks and promising not to share info with anyone outside of the agreed criteria.
* Optional: if routine checks are usually done remotely, consider meeting at least once per year including heirs to add a human element to this agreement and making heirs more familiar with the process and the fellowship. The main advantage of relying on a community over a company is that fewer people are involved, and they are better known to you.

## Example
* Alice, Bob, and Charlie have agreed to form a fellowship with a quarterly cadence and 1 week deadline.
  * Due dates are the first day of the calendar quarter (1/1, 4/1, 7/1, 10/1)
  * Send shared info in a direct Signal message back to the author (Alice’s info goes to Alice, Bob’s to Bob, and Charlie’s to Charlie). Disappearing messages must be on or manually deleted after
  * If a peer does not respond within 7 days (1/8, 4/8, 7/8, or 10/8), their dead man’s switch is executed and the peers should be prepared to execute inheritance/recovery info.
  * If a peer is obviously alive but frequently misses the 7 day deadlines the laggard can be replaced by the other participants. That peer must delete the info of the rest of the fellowship.
* Each person shares info with the other two.
  * Alice shared a sparrow wallet file (password protected) and a 24 word seed phrase for one of the keys in a 3-of-5 multisig wallet
    * bacon bacon bacon bacon bacon bacon bacon bacon bacon bacon bacon bacon bacon bacon bacon bacon bacon bacon bacon bacon bacon bacon bacon bacon
    * “My husband (or Son if my husband is deceased or incapacitated) will send you a partially-signed bitcoin transaction (PSBT) for you to sign with this key. They already have the wallet password and other keys. Check their ID/passport.”
    * **(Dead man’s switch)** Email my Husband the following message: “Hello, this is Bob/Charlie. Alice has not responded to our quarterly Badger Legacy data share. I have information to recover her Bitcoin wallet, please Signal message me at your convenience.”
  * Bob shared a 12 word seed phrase and directions for the passphrase
    * gym gym gym gym gym gym gym gym gym gym gym gym
    * Passphrase is with my lawyer Jim
    * “The wallet is native segwit with the standard derivation path. Give seed and passphrase location to my Daughter if asked. She already has this info but if it gets lost or destroyed she will rely on this group. Here is her instagram, get to know her face.”
    * **(Dead man’s switch)** Signal message my Daughter this, verbatim: “Honey, if you’re receiving this it’s because I have unexpectedly passed. Please work with Alice or Charlie if you need help recovering my Bitcoin. I am so proud of you, and love you with all my heart. -Dad.”
  * Charlie shared a veracrypt encrypted container
    * “Send this container if requested by the following emails: wife@gmail.com, son@protonmail.com, son2@outlook365.com, they will know how to decrypt the container.”
    * **(Dead man’s switch)** Post the following as a public message on Nostr:

```
-----BEGIN PGP MESSAGE-----

hQEMA/n9e56QuXkOAQgAn5t/dhVQJ+aXtGvzsENelMPdPaMVI/y2hq94fcplu7v4
qgj3lJZa5PSpO5BMM2jziuO26j9AVWSlkBiGHRJRzriqXG5BKPFQKPIBP3rvLaa6
rl4mmgrjqxTxcDqWmI3G7+9mXc/D0Kxd5EODy3730rE7w/pRkKFvuSwmybKNibtA
HfwlhCK3n30JWYEBUU7cQ0mdABl8Pb8QMGVWLiAEUpjzkLWey2aJWjZDZ03mQ3BI
F/oQ/C0KDfMgF0luCg3cvJ8tNjU3s/aUHGKC6TtmnihiKjOAu7P8aPeCaej9V+NA
n4vpeQaE3qxIiCEQEwOZ7U3dWGTcFsc3orbO9XdV99LAxQGbnAEACiDlIOqhh7v5
rghrdrtQ4mrqLE09DGRdXACmG+jQ2A1438JZewf46BVxHN+79xSShT0tFFSHZgy+
UOjBzYDxoo3o3s5nUvOWmE4nVKHjaDPaT28BEkuZLifLKSKtqlSJKAcmwIsiJHA7
xIfzRMbJ1Qzc5k60X9TAmow+NxBk02iZp/k7T1VDVAVyhGH0756XhCeqXzV+ZcwX
ZGQYfbcAgqSdQUsuPbKF5C9UYVh/Msbf9SwL3egclW72SqFVFdS29IRIGygmab8Y
ag6iz5Av4iMc5mg9TyorX7+k/veqvEwLSwlq76dkg63Qm47+AGzB40CgEhzzHklc
NoNsrVfGDIq6RKpS7gVpOYC0kEzDZGWjVL9m5xjw3t0LRHWX4/uGC2LOYUe0mWAp
3Jr7M5F/Wvgtoo5Wh4UQ1UEQUb/1+T18Ah8Uk8dovLoK+MAPqCXB8YB0r6AKGsg+
U56xOVkgf7sWuzqLo08qY28NkLqCeiOKV1s6SytQCblhzfBXa19m
=Ad2V
-----END PGP MESSAGE-----
```

In this example, each person knows they must ensure the fellowship does not have enough info to see or move funds. They must also similarly test their heirs on the info not given to the fellowship. It’s a good idea to do this with the same cadence as the fellowship itself. For example, when Bob and Charlie send Alice her Sparrow wallet file, she should download it (or have her husband and son do so) and test to make sure it opens and shows the right funds.

## Role of SD Bitcoiners
This process can be done by anyone with only the people involved knowing it exists. There may be value, however, an in impartial third party to facilitate certain aspects. These include but are not limited to:
* Maintaining this guide and updating with corrections/improvements
* Connecting people forming a fellowship, possibly with randomization
* Suggesting methods of information sharing and steelmanning trade-offs
* Mediating disputes between participants
* Serving as a holder of fellowship details
* Sending automated alerts with coreybot

Reach out to [Corey](https://corey.lol/) for any of the above.

[Github Repo](https://github.com/inpharmaticist/badgerlegacy)
