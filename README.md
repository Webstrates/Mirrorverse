# Mirrorverse

Mirrorverse is a proof-of concept system that shows how live tailoring can be technically
realized in a video conferencing interface. It builds on the Webstrates software stack consisting of [Webstrates](https://webstrates.net/), [Codestrates](https://codestrates.projects.cavi.au.dk/), and [Varv](https://varv.projects.cavi.au.dk/).



## Use

Mirrorverse can run on any Webstrates server. To setup your own Webstrates server see the [Webstrates documentation](https://webstrates.github.io/gettingstarted/installation.html).

To create an instance of Mirrorverse use the prototype ZIP file using the [HTTP API](https://webstrates.github.io/userguide/http-api.html) of Webstrates. The following link creates a copy on the public [demo.webstrates.net](https://demo.webstrates.net/) server:

> https://demo.webstrates.net/new?prototypeUrl=https://github.com/Webstrates/Mirrorverse/raw/master/prototypes/mirrorverse.zip

To create a copy on your own server replace the server address with your server:

```
https://your-webstrates-server.com/new?prototypeUrl=https://github.com/Webstrates/Mirrorverse/raw/master/prototypes/mirrorverse.zip
```




## Known Bugs and Limitations

### Using a Mirrorverse Instance in Multiple Tabs of the Same Browser Window

Due to a bug in the `localStorage` data store of Varv, Mirrorverse must not be opened in two tabs in the same browser window that share their local storage object. If testing locally, use a guest or incognito browser window instead that uses a separate local storage.

Opening a Mirrorverse instance multiple times in the same window can result in the `userManager` concept instance to be deleted.


### Room Recording Tool Unavailable

The Room Recording Tool is not available in the public release of Mirrorverse due to dependencies on unpublished code of [Videostrates](https://videostrates.projects.cavi.au.dk/).


### Fixed Versions

The versions of all [WPM](https://github.com/Webstrates/WPM) packages in the Mirrorverse prototype are fixed and will not update automatically.



## Paper ([PDF](https://pure.au.dk/portal/files/335560667/Mirrorverse_UIST_2023_authorversion.pdf))

### Abstract

How can we let users adapt video-based meetings as easily as they rearrange furniture in a physical meeting room? We describe a design space for video conferencing systems that includes a five-step "ladder of tailorability," from minor adjustments to live reprogramming of the interface. We then present Mirrorverse and show how it applies the principles of computational media to support live tailoring of video conferencing interfaces to accommodate highly diverse meeting situations. We present multiple use scenarios, including a virtual workshop, an online yoga class, and a stand-up team meeting to evaluate the approach and demonstrate its potential for new, remote meetings with fluid transitions across activities.


### Video

[![Mirrorverse Video](https://img.youtube.com/vi/ATAgvKrWZxg/0.jpg)](https://www.youtube.com/watch?v=ATAgvKrWZxg)



### Citation

> Jens Emil Grønbæk, Marcel Borowski, Eve Hoggan, Wendy Mackay, Michel Beaudouin-Lafon, and Clemens N. Klokmose. 2023. Mirrorverse: Live Tailoring of Video Conferencing Interfaces. In Proceedings of the 36th Annual ACM Symposium on User Interface Software and Technology (UIST ’23). Association for Computing Machinery, New York, NY, USA. DOI: https://doi.org/10.1145/3586183.3606767


### BibTeX

```BibTeX
@InProceedings{Mirrorverse2023,
    author    = {Grønbæk, Jens Emil and Borowski, Marcel and Hoggan, Eve and Mackay, Wendy and Beaudouin-Lafon, Michel and Klokmose, Clemens N.},
    title     = {Mirrorverse: Live Tailoring of Video Conferencing Interfaces},
    year      = {2023},
    booktitle = {Proceedings of the 36th Annual ACM Symposium on User Interface Software and Technology},
    series    = {UIST '23},
    doi       = {10.1145/3586183.3606767}
}
```
