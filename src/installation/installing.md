# Installing Pi Relay

Pi Relay is made for Raspberry Pi and uses an e-paper display to show real-time information about your relay's activity.

To start the installer, enter:

`curl --proto '=https' --tlsv1.2 -sSfL https://install.pirelay.computer | bash`

## Choose Your Relay Type

After the install script begins, you'll choose the kind of relay you want to configure. Making the right decision for your installation environment will be necessary.

Before proceeding, read about the [different kinds of relays](relay-types.md).

For this guide, we'll choose a middle relay.

## Configure Relay Information

You need to set a few variables before your relay can go online.

### Relay Nickname

We automatically generate a nickname that looks like `pirelay231009`. Avoid using special characters, spaces, or long names if you change it.

### Port

Your relay needs a port to make itself available to pass information. You must also forward this port if you're running the relay from home. If you don't know how, search for your router's instructions. 

We pre-fill this option with port 443, the port used for secure HTTPS web requests. The default port that Tor uses is 9001, but this can be easily blocked. To get around port censoring, we chose 443 because blocking this would mean blocking much of the internet.

### Monthly Bandwidth Quota

This is your "accounting max". To make it easy, we set this up as a monthly quota. Middle relays are required to share a minimum of 200 GB per month.

### Bandwidth Limits

You'll set your bandwidth limit and burst rates. Tor recommends at least 2 MB/s, with a 4 MB/s burst. These values are entered by default for you.

### Contact Info

You can optionally add your name and email address so Tor can notify you if your relay ever goes down. There's a default value entered for you, but consider adding an address you have access to.