---
layout: default
title: Seeds
nav_order: 4
---

# Generating your seeds
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Intro

First, a reminder of where you should be in the process by now.
You should now have one digital note in Bitwarden containing:

```
PW: your_wallet_password
PF-HW: your_hardwarewallet_passphrase
PIN-Coldcard: hint_pin_coldcard
PIN-Trezor: hint_pin_trezor
PIN-Ledger: hint_pin_ledger
```

If everything looks good, it's time to generate your private seeds!

This is the meat on the bones, the most important thing of your setup. So, a few things to keep in mind when generating your seeds. This is valuable information. If someone gets access to your seeds, they get access to your funds (they'll need 2 of 3 seeds in our multi-sig setup). A lot of devices are “spying” on us in one way or the other today. If possible, generate all seeds in a room where other electronic devices connected to the internet are turned off. Make sure that your actions aren´t visible from windows or doors and that no home security camera records your actions.

Try to keep smartphones turned off and/or in another room during the process. They are hard to secure and can record sound/video without you noticing (computers can of course do the same). Generally, use your common sense to make sure that nothing can record your actions.

## Generating the seeds

You should have the following at hand:

* Your Coldcard
* Your Trezor 
* Your Ledger
* 3 different notes to write your seeds and PIN-codes on (you can use the paper often shipped with the hardware wallets or use your own paper). On two of the notes you're going to write down two passphrases as well. So, might be good if there's some extra room.

Before starting, make sure to update the firmware on the hardware wallets if you don't have the latest version. Follow the instructions for each different manufacturer:

* [https://coldcardwallet.com/docs/upgrade](https://coldcardwallet.com/docs/upgrade){:target="_blank"}
* [https://wiki.trezor.io/User_manual-Updating_the_Trezor_device_firmware__T1](https://wiki.trezor.io/User_manual-Updating_the_Trezor_device_firmware__T1){:target="_blank"}
* [https://support.ledger.com/hc/en-us/articles/360002731113-Update-device-firmware](https://support.ledger.com/hc/en-us/articles/360002731113-Update-device-firmware){:target="_blank"}

The logic behind using 3 different hardware wallets is that if a fatal flaw was found in one product, your funds would still be safe. If that happens, simply move your funds to a new multi-sig contract and replace the compromised product.

Coldcard, Trezor and Ledger is three of the most reputable names in this space. So, selecting one wallet from each seems reasonable.

Follow the setup procedure recommended for generating a single seed by each manufacturer. For Coldcard, we will be using it "cold" with an SD-Card to move information between the Coldcard and the computer. Don't worry about multi-sig or passphrase at this point. We will take care of that later.

If you already have a seed that you know have been generated in a secure way, you could use that (say you are using an old device). The different passphrase and the multi-sig combination will break any links to any other funds stored at the device.

If this is the first time using a specific hardware wallet, I would recommend setting up a "dummy wallet" at first to get a feeling for the process. Then wipe it before creating the real wallet.

At the end you should have one seed from each wallet. Mark the seed generated by the `Coldcard` with `Seed A - Coldcard` , the seed from Trezor with `Seed B - Trezor` and the seed from Ledger with `Seed C - Ledger`.

Protect the devices with the PINs you created in the last step and add the full PIN to the corresponding note (So `Seed A - Coldcard` with `PIN Coldcard` etc). On the Coldcard, the PIN consists of two parts. Split the PIN you selected in two parts and make sure you'll notice how you split it on the note.

## Add information

Before moving on, we are going to add some information to the notes we wrote our seeds on. Space could be an issue here, but try to find some space somewhere on the note (could be the backside). If it's not possible use a separate note and staple it to the note with the seed at the end of the process.

Start by marking each seed with:

`hodl-guide.github.io (v2.0), multi-sig 2 of 3`

That should give enough information for someone else to do a search online, find the guide and hopefully be able to follow the steps in case of an emergency.

We are now going to add the `PW` and the `PF-HW` to two of the notes. Make sure to write clearly! 

On `Seed A - Coldcard`, somewhere on the note add the PW: `PW: your_wallet_password`

On `Seed B - Trezor`, somewhere on the note add `PF-HW: your_hardwarewallet_passphrase`

That's it, you now have all the necessary information to create your wallet. We'll go into exactly why we did this in [Storage](hodl-guide_50_storage.md){:target="_blank"} later on.

Store all generated information in a secure way during the rest of the process (don't leave your notes lying around visibly).

Move on to creating the wallet.

---
Next up: [Create the multi-sig wallet >>](hodl-guide_40_multi-sig.md)
