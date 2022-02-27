# WARNING

**WARNING(1)!** This repository contains things that are normally bad ideas.
It contains an aggregation of things that are probably bad ideas in any civil, acceptable
circumstance where a reasonable social contract is in place. Moreover, none of the
information is vetted. **ONLY** the article that appears imediately below was written by
me. **USE IT AT YOUR OWN RISK.** ALL, **I MEAN ALL** of this advice is
**OBJECTIVELY DANGEROUS.** It is presented solely for educational purposes in a world that
continues to present us all with objective dangers. It is not be taken lightly.

**WARNING(2)!** This document is a work-in-progress. In particular, the tools required
**simply don't exist yet**, I have to make them. We need modified versions of several
Android and Desktop applications to operate this network safely, which is going to take
a couple of days for me to do. Sorry. Wish I could do it faster. Read what's here maybe
and help me finish if you can. I understand if you can't.

**Consider yourself warned.**

# Wouldn't it be scary if you could build a surveillance system out of burner phones?

Boy, it sure would be a shame if surveillance at scale was very easy for regular people
to pull off, wouldn't it? Like pretty much everything is always searching for a connection
these days, it would be pretty scary if a bunch of cheap, off-the-shelf hardware that can
readily be acquired over-the-counter could be turned into an ad-hoc means of monitoring a
person or person's movement through an area.

Perhaps an area that they **definitely should not be in.** Doing things they **definitely**
**should not be fucking doing.**

Take the hint? Good, now here's how to be the worst version of Batman with stuff that you
can probably find or salvage on the cheap, even in emergencies.

## If you're reading this, you have goals

Among may be:

- Stay alive!
- Gather Intelligence!
- Repel Invaders!
- Profit?

I'm going to try and help you with the first two, and toss out some suggestions for the third.
Then I'm going to suggest that you consider carefully how you do the fourth. Let's break down
the tasks relevant to this operation for each of those goals.

## Terms

- **Device Scanner:** A modified android device which is used to capture information about the environment
 using the sensors available to the device.
- **Device Controller:** A laptop which is used to connect to a large number of Android Device Scanners,
 which are used to aggregate signals and turn them into useful information.
- **Device Network:** A large group of Android Device Scanners under the control of a laptop Device Controller, 
 which is under the control of a Device Operator.
- **Device Operator:** A person operating a device network.
- **Hidden Service:** A system for hosting online service using a third-party intermediary, often in another
 legal jurisdiction, in order to evade perfunctory incarceration when communications are restricted
 by an oppressive regime or hostile threat.
- **Belligerent threat:** These are people trying to capture, maim, or murder you, who may gather information
 about your sensor network in order to identify and harm you.
- **Forensic threat:** These are people trying to identify you post-facto in order to suppress your resistance
 in the future. They are also trying to capture, maim, or murder you, but they will wait longer to do so
 successfully.s
- **Beacon Frame:** A wi-fi signal periodically emitted by all modern phones and most other devices,
which indicates to other devices that it is present in the area.

## Tools

In order to accomplish this, you'll need to collect some tools:

**Hardware:**

1. **[Android devices](https://en.wikipedia.org/wiki/List_of_Android_smartphones):** Get as many of these
as you can find. We will use these to build our sensor network, and at a certain point will leave the
operator's hands to be planted in a location where it will fulfill it's goal of running

- **[According to cursory research, these phones are popular in the Ukraine](https://www.appbrain.com/stats/top-android-phones-tablets-by-country?country=UA):**
I copied this list to UKRAINE_PHONES.md in this repository.
- You should also get as many USB cables as possible, to use for charging the phones and attaching
them to permanent power supplies. Changing batteries is a risky operation best avoided, lives will be
lost if we're too dependent on batteries.

2. **[Laptop PCs](https://en.wikipedia.org/wiki/Laptop):** It is less critical that you have many of these,
but you should have a few, in good condition, with working batteries and up-to-date Operating Systems.
If you can secure a Linux desktop I would recommend using that, but it is of the utmost importance that
the operator be familiar with the security of the laptop's Operating System. These will be used to
aggregate information as the "Device Controller."

3. **[Information Sources](RUSSIA_PHONES.md):** I'll provide a few to get you started, but in many cases
you'll need to build your own. You will be looking for "Device Fingerprints" which match Russian tech.
The FIND3 software below is what we're using to accomplish this task.

**Software:**

- **[Find3 Android Scanner Application](https://github.com/schollz/find3-android-scanner):** We use this
to scan for passive signals from nearby wi-fi devices, and collect information from those signals.
- **[Modified GoRAT(UNFINISHED!) See warning 2.](https://github.com/eyedeekay/GoRAT):** We use this to manage
large numbers of Android devices from a single laptop.

You should **DOWNLOAD** this software and keep it nearby on a removable storage device so you don't need
to download it repeatedly. You should share your downloaded copies with other operators who you trust.

### Staying Alive

I dunno, I've never been in a war but I'm trying to contribute. If I were in your shoes, job
one would be stay the fuck alive. You do it for your family, you do it for your country, you
do it for you. Dying for your country isn't the goal. Defending it successfully is.

Now that I'm done stating the painfully obvious, maximizing your chances of staying alive means
considering the threats to your existence. This is called "Threat Modeling." It can be a
challenging, multifaceted process, and you're probably already doing it. The reason I'm touching
this point is because I'm about to instruct you in how to build something dangerous in your
own neighborhood, and do the kind of hacking I wouldn't dare try in my own country. If you're my
target audience, you are already at extravagantly high relative risk because you're being
invaded, and that justifies doing dangerous things close to home. Bottom line? You must understand
the risks of being the operator of a massive surveillance network.

The upside is that if you can manage the risks, then you can use this system to help you manage
other risks. You can tell where devices are, gather information on unknown devices, and expand
your view of your surroundings, allowing yourself more time to make better plans for counter
attack or tactical movement.

#### You need to account for

1. Your adversary **will** eventually recover **multiple** Device Scanners from your network as troops
advance.
2. You **are** already being asymmetrically surveilled by invaders.
3. Job one is to make sure that the compromise of a device is insufficient to compromise the device
operator.
4. Job two is to make sure that the compromise of a device is insufficient to compromise the
operation of the device network.

#### Your threats appear to be

Primarily **Belligerent** in nature.

##### Defending a Device Controller from a compromised Device Scanner

WHY(TODO): Device Controller is under control of device operator

- Physically conceal the **Device Controller**: TODO
- Attach the device controller to an external power source, wall outlet, battery, or both: TODO
- Make extracting the device from the concealed location unpleasant, difficult, or dangerous: TODO
- Monitor device actively and remote-wipe: TODO

### Gathering Intelligence

Your goal is to gather sensor information from a large number of phones, and interpret it, rapidly
when that sensor data indicates the presence of data.

### Repelling Invaders

A phone can neither fire nor stop bullets. But since we're expecting them to become targets, then it
may make sense to defend them in ways which allow the defenders to keep their distance and thoroughly
destroying the phone.

### Profit?

When the interlopers are removed, the system you have built does not lose it's power.

- See also: [Passive Device Fingerprint Collection app FIND3, chosen for this purpose](https://github.com/schollz/find3-android-scanner)
- See also: [Passive Frame Collection App PandaCollector](https://github.com/CoreTheGreat/PandaCollector)
- See also: [Passive Frame Collection App AndroidBeaconApp](https://github.com/ashishshettyb1993/AndroidBeaconApp)
- See also: ![This picture, alledgedly of Voldomyr Zelensky's enormous balls](https://abcwipeout.fandom.com/wiki/Big_Balls?file=Bigballs-2.jpeg)
