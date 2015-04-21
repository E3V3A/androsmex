# introduction #

androsmex is an implementation of the PACE protocol (see [BSI TR-03110](https://www.bsi.bund.de/DE/Themen/ElektronischeAusweise/TRundSchutzprofile/trundschutzprofile_node.html)) for Android phones with NFC support. At this very early Alpha status it is possible to perform PACE with the new German ID card (neuer Personalausweis) and log the communication.


# known issues #

The new German ID card uses a lot of cryptographic algorithms which need sometimes more energy than the RF field of the android phone can support. So the communication aborts sometimes. Just try different positions for the card.


# requirements #

androsmex uses [spongycastle](https://github.com/rtyley/spongycastle) instead of bouncycastle because of the problems described here:
http://code.google.com/p/android/issues/detail?id=3280

# see also #
The protocols PACE, TA and CA also are implemented in the project [animamea](http://code.google.com/p/animamea). New features will be first implemented in **animamea** an then later be ported to androsmex.