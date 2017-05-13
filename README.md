# PracticalD
TutorialD is a relational database language that supersedes SQL

This github page is for ideas, and when time permits, code, to implement practical implementations of TutorialD

Key ideas:
* DuroDBMS already exists. Simple turn it into a DLL to load into other languages, not just TCL/TK
* or if not a DLL, then use SimpleIPC to communicate with DuroDBMS and send strings to it and other commands. If not using SimpleIPC then use other IPC mechanisms (inter process communication)
* Rel project exists too but is written in Java. Probably better to use DuroDBMS codebase as it is reusable C code that can be statitically or dynamically linked into other languages and programs
* GoLang can load a durodbms/duro DLL into it, theoretically.. Figure out ways to make golang communicate with DuroDBMS
* DuroDBMS/TutorialD could also use sqlite optionally, as a storage mechanism instead of the Berkley database, in order to make it easier to deploy durodbms without installing Berkley database.  Truly relational databases do not require rewriting your own full DB and can make use of existing databases, but some people will want to roll their own without reusing existing technology
* todo: try making durodbms dll or IPC system that can be loaded into: golang, rust, fpc, delphi, nimrod, python to talk to durodbms from multiple languages/exe's/elf's
* make a demo game that tracks an airplane shooting down objects in the video game and store its bomb/kill count in a truly relational db :-)

