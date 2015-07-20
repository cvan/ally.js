
# ally.js Goals

The ultimate goal is to make the development of apps adhering to [WAI-ARIA](http://www.w3.org/TR/wai-aria/) a breeze. The ultimatest™ goal is to make this library obsolete by lobbying the W3C and browser vendors into supporting the basic tools provided by ally.js. (One may dream…)

Applications have to deal with quite a number of different issues to get to a state we may call "accessible". There's the issue of *maintaining the focus*, a subset of providing *keyboard navigation*. Then there's [WAI-ARIA](http://www.w3.org/TR/wai-aria/) to provide help the browser provide the operating system's Accessibility Infrastructure with the necessary details.

Documents like [WAI-ARIA Authoring Practices](http://www.w3.org/WAI/PF/aria-practices/) try to explain what needs to be done, but even though the documents have been "dumbed down", they're still too convoluted to allow quickly understanding things. With `ally.js` I want to take that english language document and turn it into generic, reusable JavaScript.

It does not make sense to implement the same things over and over again, which is why `ally.js` is designed in a way that while allowing simple and direct integration (like jQuery), exposes every function individually. The modularity is paramount for preventing application and library authors from copy-pasting code, or worse, rolling their own flawed implementation. While ally.js is not perfect (it's software, it's written by me, …), I want to make this *the place we focus our efforts* - much like has happened for the DOM by way of jQuery.

With ally.js v1.0.0 I've laid the *ground work* for a library solving the "stupid problems" (like "what is focusable?"), so developers won't have to anymore. Here are the topics I'd cover next (not necessarily in that order) and would love your support:

* [x] simplify managing focus
* [ ] simplify basic keyboard interaction (`enter`, `escape`, `space`) 
* [ ] implement a DOM based interface to simplify handling [WAI-ARIA state attributes](http://www.w3.org/TR/wai-aria/states_and_properties) (along the lines of [IBM-Watson/a11y.js](https://github.com/IBM-Watson/a11y.js))
  * easily creating unique-IDs for linking elements e.g. `<label for="uniq-123">…</label><input id="uniq-123">`
  * toggling states
* [ ] implement a keyboard command abstraction that maps the keyboard interactions suggested by [WAI-ARIA Authoring Practices](http://www.w3.org/WAI/PF/aria-practices/) (e.g. [Listbox](http://www.w3.org/WAI/PF/aria-practices/#Listbox)) to [Indie UI Event Triggers](https://w3c.github.io/indie-ui/indie-ui-events.html#triggers)
* [ ] implement the corresponding [Indie UI Event Actions](https://w3c.github.io/indie-ui/indie-ui-events.html#actions) against DOM elements depending on their `role="…"` attribute

---

For the time being ally.js is developed along side my actual work projects and features get added to ally.js once they become necessary to them. Of course you're welcome to contribute whatever and however you can. I don't bite, promise.
