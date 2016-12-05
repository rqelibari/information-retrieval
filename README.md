# Information Retrieval
Little projects written in C++ for my "information retrieval" class.

## What is Information Retrieval about?
[Information retrieval][1] (IR) as I am learning it is the science about better
filtering. Generally spoken you normally have a (huge) dataset, from which you
want only a subset, which depends on your intention. Google for example has a
billion Websites as its dataset, but only wants the ones, which fit your search
query best. An email application has a lot of emails as its dataset but only
wants to accept non-spam messages.
Retrieving a subset is also known as filtering. So:

> IR enables software to build
this filter by using [metadata][2] which inherently belongs to the dataset.

[1]: https://en.wikipedia.org/wiki/Information_retrieval
[2]: https://en.wikipedia.org/wiki/Metadata

## Setup
### Prefered way
1. Add this repository as a submodule to your current repository
(e.g. to `vendors` subfolder):

```
> cd  <your-git-repository>
> mkdir -p vendors && cd vendors
> git submodule add https://github.com/rqelibari/cpp-project-template.git
```

2. Link Makefile to your repositorys root and run `make init`:

```
> cd <your-git-repository>
> ln -s ./vendors/cpp-project-template/Makefile ./
> make init
```

### Other ways
1. Download this repo as a zip and unpack it to `REPO_DIR`. Alternatively, you
can clone this repo to `REPO_DIR`.

2. Run the followin code:

```
> cd REPO_DIR
> make init
```

If you cloned this repository then you should change the remote url now:

```
> git remote set-url --push <url-to-your-remote-repo>
```

## Projects
### Fuzzy Search
Implement a fuzzy search tool. Read a file full of words and lets you
then search for those words. So what's it all about?
You can actually make typos and it still will find the right words.

### Completion Websearch
A standard client server architecture application. Consists of a webserver and
an according webservices which enables a user to search for lines in huge files.
If the file contains geodata the webservice shows the result on a map.
Topics touched by this project are:
*Client-Server Architecture, Webapplication Modeling, Responsive Webdesign, Server
Security*

Technologies used:
[Sockets][3], [HTTP][4], C++, Javascript, HTML, CSS

[3]: https://en.wikipedia.org/wiki/Network_socket
[4]: https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol
