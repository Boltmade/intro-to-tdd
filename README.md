# Intro to TDD

To get started, make sure you have [VirtualBox](https://www.virtualbox.org/)
and [Vagrant](https://www.vagrantup.com/) installed. Then, clone this
repository, cd to the folder, and run `vagrant up`.

Once that's done, `vagrant ssh`, cd to `/vagrant` and run
`ruby calculator_test.rb`. You should see output that looks like this:

```
# Running tests:



Finished tests in 0.000756s, 0.0000 tests/s, 0.0000 assertions/s.

0 tests, 0 assertions, 0 failures, 0 errors, 0 skips
```

If that's what you got, you're good to go!


# Doing the Exercise

The exercise is called "String Calculator" and is based off of the information
found [here](http://osherove.com/tdd-kata-1/).

All of the steps can be found in [requirements.md](requirements.md). Typically
you would take one, write the test, write code that passes the test, refactor,
and then move on to the next one.

The vagrant box is setup for ruby development, but of course the requirements
are not language specific and therefore can be done in any language.

# The Presentation

The presentation PDF is located at [presentation.pdf](presentation.pdf), or
on [SpeakerDeck](https://speakerdeck.com/ericroberts/intro-to-tdd). PDFs are
not very friendly to GIFs, so it does look a little weird. It was written in
Markdown and presented using [Deckset](http://www.decksetapp.com/). The original
Markdown file can be found in [presentation.md](presentation.md).
