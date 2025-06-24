---
layout: page
title: Contacts
---

If you would like to keep informed about new events and initiatives related to EUD, join the EUD mailing list!

Please send an email to <listserv@listserv.cnr.it> by including in the body (not in the subject) this sentence: `Subscribe EUD name surname`.

You can then send your messages to the mailing list just by writing to <EUD@isti.cnr.it>.

{% assign chair =  site.data.steering-committee | find: 'chair', true %}
For any further information please send an email to the Steering Committee chair: [Antonio Piccinno](mailto:{{ chair.email | encode_email }})
