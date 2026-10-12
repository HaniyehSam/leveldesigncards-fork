# Level Design Cards

Brainstorming-cards related to **Level Design**.

- arrange / think / discuss!
- read between the cards!

Card data (XML files) to work together with https://github.com/csongorb/cardsimulator.

## Structure

This repository holds **content only**. Everything that displays the cards comes from [cardsimulator](https://github.com/csongorb/cardsimulator), included as a git submodule (pinned to a commit).

- `cards/cardset.xml`: title, repository and public address (used by the QR codes in PDFs)
- `cards/cardCategories.xml`, `cards/cards.xml`: the cards
- `texts/`: documents linked from the cards
- `index.html`: tiny loader, identical in every card set
- `.github/workflows/deploy.yml`: publishes the site to GitHub Pages on every push to `main`
- `cardsimulator/`: the simulator (submodule)

Run locally with any static web server (the XML can't be loaded from `file://`): `python -m http.server`, then open http://localhost:8000/.

Update the simulator: `git -C cardsimulator pull origin main`, then commit the changed `cardsimulator` pointer.

## Changelog

### Todos / Ideas / Bugs

### Release 3.0 (Work in Progress)

- restructured the main architecture, repository separated into
	- cardsimulator
	- leveldesigncards (that includes cardsimulator as submodule)
- some other links updated
- repository is now content only: new card table from `cardsimulator`, tiny loader `index.html`, `cards/cardset.xml`, GitHub Pages deploy workflow
- removed `xmlfiles.html` (no longer needed with the deploy workflow)
- replaced all broken gamasutra.com links with working gamedeveloper.com links
- new cards
	- lonely maintains: downhill
	- level data structure

### Previous Versions

See: https://bitbucket.org/csongorb/porncreator/src/develop/01_input/leveldesignporn/

## Credits

- **Csongor Baranyai**  
	- csongorb (at) gmail (dot) com  
	- [csongorb.com](http://www.csongorb.com)

Thanks to all the **universities / schools / institutions** where I had the opportunity to teach courses, supervise students and projects, and refine the idea of the brainstorming cards. And of course a huge thank you to all the **students** who have contributed with all their comments and critiques... and who have tolerated my experiments.

Additional design / coding:

- **Christoph Maureder**
	[christophmaureder.me/](https://christophmaureder.me/)

## License

[![Creative Commons License](https://i.creativecommons.org/l/by-nc/4.0/88x31.png)](http://creativecommons.org/licenses/by-nc/4.0/)
This work is licensed under a [Creative Commons Attribution-NonCommercial 4.0 International License](http://creativecommons.org/licenses/by-nc/4.0/).

All other media (images, software, etc.) remain the property of their copyright holders.
