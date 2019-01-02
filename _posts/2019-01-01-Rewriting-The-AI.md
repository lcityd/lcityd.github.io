---
  layout: post
  title: Rewriting The AI
  tags: 
  categories: 
---

So, I was originally going to rewrite the original paragon personal assistant, but I've decided to simply start with the base code, and redisgn it with not only a multiplatform design in mind, but a multi user/loose design in mind. 

Some changes that are going to be made (hopefully):

- Relative directory names assigned at setup
- Preconfigured database downloads, along with prompts to ask for downloads if the databases don't exist (which means a comprehensive 404/400 exception process)
- a requirements.txt file and a linux.sh and a windows.sh for the various install methods, available on the github. If one wants to compile and setup the code by hand, theyre more than welcome to do that.
- Work on a step by step guide for any account information that might be needed in order to set up things for wolfram, or any other thing. 
- Check for certain programs installed at the runtime of the installer, and configure the code to run with those software included, along with any functionality.

So, as one can see, there's a lot of new features being sought after, along with the major overhauling of the code and the libraries. For example

- Speech Recognition driver overhaul (look into writing the speech recognition in C++, as it allows much faster runtimes)
- Provide an option for the video based libraries (Person Identifier, object detector), along with optimization of those algorithms (remove the windows, so that they don't have to render in realtime)
- Speech Synthesis library, only thing that needs to be done is further increase the accuracy, and increase the speed. This should be easy, as it uses the original tacotron algorithm released by google back in 2016-2017.

So, I'll keep you guys updated and informed on the status of the code, but keep in mind I'm also working on an operating system, which is booting at the moment, I've got to get a package manager running, I'm going to use dpkg, wget, and apt, for handling downloads. 
I also still have this website to maintain, not that this is a bad thing, but I might potentially be on the path to too many projects, which I don't dislike, but things such as my school grades and my social life may suffer as a result, but at least I'm occupied.
  -kalbot