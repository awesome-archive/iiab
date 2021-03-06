==============
Network README
==============

This is run by Ansible after it has installed the core of Internet-in-a-Box (IIAB) and its apps/services.

Specifically, this 'network' role is run:

- automatically during IIAB installation, after /opt/iiab/iiab/iiab-install has run `Stages 0-to-9 <..>`_ (thanks to `iiab-stages.yml <../../iiab-stages.yml>`_)
- automatically by IIAB's Admin Console (http://box/admin) if you click ``Configure`` menu -> ``Install Configured Options`` — this is similar to the above, but only runs Stage 0, then Stage 4-to-9, and then finally this 'network' role/stage (thanks to `iiab-from-console.yml <../../iiab-from-console.yml>`_)
- or manually, if you run ``cd /opt/iiab/iiab`` then `./iiab-network <../../iiab-network>`_ (which is much the same as running ``./runrole network``)

Many IIAB networking questions can be answered in these 2 documents:

- `IIAB Networking <https://github.com/iiab/iiab/wiki/IIAB-Networking>`_ is a high-level summary, that reviews IIAB's 3 modes of operation distinguishing WAN from LAN, `common ports <https://github.com/iiab/iiab/wiki/IIAB-Networking#list-of-open-ports--services>`_, DNS name resolution and some common customizations.
- http://FAQ.IIAB.IO includes answers to common questions like:

  - How do I provide Wi-Fi (wireless) to all my kids?
  - Can I create a Wi-Fi hotspot using an old laptop?
  - How do I change the wireless network name?
  - Can I name my server something other than http://BOX.LAN ?
  - How do I set a static IP Address?
  - Any other networking tips?
