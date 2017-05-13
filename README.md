# PracticalD
TutorialD is a relational database language that supersedes SQL

This github page is for ideas, and when time permits, code, to implement practical implementations of TutorialD

Key ideas:
* DuroDBMS already exists. Simply turn it into a DLL to load into other languages, not just TCL/TK
* or if not a DLL, then use SimpleIPC to communicate with DuroDBMS and send strings to it and other commands. If not using SimpleIPC then use other IPC mechanisms (inter process communication)
* Rel project exists too but is written in Java. Probably better to use DuroDBMS codebase as it is reusable C code that can be statitically or dynamically linked into other languages and programs
* GoLang can load a durodbms/duro DLL into it, theoretically.. Figure out ways to make golang communicate with DuroDBMS
* DuroDBMS/TutorialD could also use sqlite optionally, as a storage mechanism instead of the Berkley database, in order to make it easier to deploy durodbms without installing Berkley database.  Truly relational databases do not require rewriting your own full DB and can make use of existing databases, but some people will want to roll their own without reusing existing technology
* todo: try making durodbms dll or IPC system that can be loaded into: golang, rust, fpc, delphi, nimrod, python to talk to durodbms from multiple languages/exe's/elf's
* make a demo game that tracks an airplane shooting down objects in the video game and store its bomb/kill count along with all the important statistics/data about what was bombed (building addresses, etc.) in a truly relational db :-)
* TutorialD language syntax: the language is a bit heavy to use. Figure out ways to make the language lighter on the hands possibly and more precise than its current verbose state? This needs to be looked into, as one reason people use OOP (object orientation) is for easy access to data with dot notation (i.e. Ruby) without having a huge heavy language just to do simple things. SQL already suffers from being a bit heavy, and TutorialD also does, although it has made some improvements on some areas such as not requiring SELECT keyword

At the moment this github page is just a start of ideas, when I get time to experiment with some code it will be uploaded to this project page.  Right now working on IPC and other areas of work, which, ironically relates to the practicald ideas anyway
