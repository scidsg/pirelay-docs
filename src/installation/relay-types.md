# Types of Relays

After the install script begins, you'll choose the kind of relay you want to configure. Making the right decision for your installation environment will be necessary.

## How Tor Works

First, let's understand how Tor works before choosing the kind of relay to use. [Tor](https://torproject.org) offers online anonymity by hiding information about your digital footprint, including your IP address, browser size, and operating system. 

Think back to your preschool days when you wanted to send a secret "I <3 U" note to a crush. You asked your bestie to deliver it, ensuring your crush remained clueless about the admirer. In this analogy, your friend acts as a relay for you. But instead of the note going from you to your bestie to your crush, it goes from you to three random volunteers around the world, who you don't know but will deliver the message.

## Entry Relays

In your chain of three volunteers delivering your note, the first person is the entry relay. The Tor network itself chooses relays based on factors including stability and performance. The entry doesn't know the destination address.

## Middle Relays

A middle relay is the second person in the chain. They don't know who you are, and they don't know who your crush is - they're simply a middle-person. 

⭐️ If you operate a relay from home, you should only choose a middle relay.

## Exit Relays

Exit relays are the last step in the chain, and will request the website on your behalf. They don't know who you are but know who your crush is. Operating an exit relay should take extra consideration and should _never_ be operated from home.

Here's a real example of why you shouldn't operate an exit from home: back in 2019, [Trump's Justice Department demanded 1.3 million IP addresses of the people who visited a Trump protest website](https://arstechnica.com/tech-policy/2017/08/feds-demand-1-3-million-ip-addresses-of-those-who-visited-trump-protest-site/). Why did they want the IP addresses? What if you never visited the site, but it looked like you did? Could you potentially get in trouble? 

If you run an exit relay, it will appear that _YOUR_ IP address is the one visiting the site.

So if the teacher catches you handing the note, it will look like it's from you. 

Again, never operate an exit relay from home. Businesses and public institutions like libraries and universities - who can donate high-speed internet and have enough money to afford legal council if needed - should only consider this option.

## Bridge Relays

Bridge relays are a special type of relay. Sometimes, the Tor Network can be blocked completely. When this happens, bridge relays are the ones who become the entry. You can share your bridge address for someone to plug into Tor Browser, or Tor can share it automatically for you.  

This person is the silent helper who will step in if all else goes wrong. They'll ensure the note is discretely delivered.