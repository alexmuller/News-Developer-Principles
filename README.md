# BBC News Developer Principles

Culture is the sum of everyone's attitudes and actions.  We need to model the behaviour we want to see in one another.  Listed below are the principles that we hold each other up to.

## We encourage learning

We value learning, community and trust.  We try to work with each other as openly and collaboratively as possible.

 * DO NOT disregard a person because they don't understand a subject.  Everyone's skillset and capacity for learning is different.  You MUST cater for different levels of understanding with the people you work with.

 * DO be open about what you know and understand.  We work in a search economy rather than a knowledge economy.  The knowledge expected for us to do our jobs is too large for one person.  It's better for you to say that you don't understand something, or ask a person for clarification on what they mean, rather than to hide your unfamiliarity with a subject.

 * You MUST actively attempt to learn about all the different codebases, systems and tooling that the development team use on a daily basis.  While we don't expect anyone to know everything, we do expect you to have the ability and capacity during the day to learn how something works.  Add time into estimating tasks for learning what you are going to do.

 * You MUST actively try to help other people learn how things work.  DO NOT store knowledge for yourself.  If you learn something, document your findings to help others get up to speed, offer help to others.

## We strive to be as objective as possible

People are complicated. You should expect to be misunderstood and to misunderstand others; when this inevitably occurs, resist the urge to be defensive or assign blame. Try not to take offense where no offense was intended. Give people the benefit of the doubt.

 * DO NOT be precious.  You MUST be open to other ways of thinking.  We are more interested in the correct opinion rather than a person's own opinion.  Technology moves fast, "Because that's how we've always done it" is not great reasoning.  And while skepticism is healthy, it must always be friendly.  Assertions should be made with evidence as much as possible, and try not to think of an opinion as yours.

## We take the performance of the website really seriously

Performance is a key feature of the site, the faster the site the happier the users.

 * You MUST think about how every change to the site impacts on the performance of the site.

 * You MUST consider the loading order of assets onto a page.  We value perceived performance over actual performance, so while increasing asset size doesn't immediately have a negative impact on user happiness, delaying the time to glass on a page will do.

 * You MUST NOT arbitrarily use libraries or new functionality on the site.  We value user convenience over developer convenience.  So if a JS library makes your job easier but increases the load on the page, don't use it.  Seek opinion from the entire department before deciding.  Do not cut performance corners to meet a product deadline as ultimately this will cause an accumulative effect of slowing the site down over a number of features.

 * You MUST only load into the page what you are going to use.  Do not stuff JS/CSS into the global packages that get downloaded on every page.  It may be convenient for you and decrease development time, but ultimately you are hurting the product.

## We practice progressive, mobile first responsive web design

The key to building modern, resilient, progressive sites doesn’t lie in browser technologies or frameworks; it lies in how we think about the task at hand; how we approach building from the ground up rather than the top down.

 * You MUST always prioritise smaller screens over larger ones.  This should happen when discussing designs, writing test scenarios and developing JS/CSS.  Layering a larger screen design onto a smaller screen design is technically simpler than trying to take a large screen design and then forcing it to work on small screens.  Thinking in a "mobile first" fashion will help you to solve the hard problems first.

 * You MUST create a basic experience that works on all browsers first.  By supporting all browsers by providing a base experience using simple HTML/CSS, we can then prioritise for modern web browsers using a rich, JavaScript experience.  Techniques like "cutting the mustard" and progressive enhancement means we can use cutting edge technologies that only work in modern web browsers.

Further reading:

 * [Cutting the mustard](http://responsivenews.co.uk/post/18948466399/cutting-the-mustard)
 * [Where to start?](https://adactio.com/journal/9963)

## We practice test driven development

We value high quality code, refactoring and bug free production environments.  A test driven development approach enables this.

 * You MUST write tests for code that goes to production.  The BBC News codebase is large and complex.  Tests ensure that we haven't broken everything.

 * Prototypes MUST not make their way to production.  While its completely legitimate to create prototypes to explore an idea or solution.  Once you've worked out how to make something, you should then go back and write unit or integration tests that are then used to make a robust, production alternative of your prototype.  We do not cut corners to reach deadlines.

 * Developers MUST browser test their code.  The web is not a platform, so don't think that the code is complete if it works in Chrome.  Testers role are to put a SECOND pair of eyeballs with manual tests.  It's not their primary responsibility that the code works in browsers other than Chrome.

Further reading:

 * "Responsive News testing principles"(https://github.com/BBC-News/responsive-news/wiki/Explain:-Testing)

## We value automation as much as possible

Automated process saves time and avoids unintended errors.  We encourage developers to spend time learning how to automate because it also exposes us to different kinds of development.  We respect our developers by giving them the responsibility to own their own processes.

 * We want developers to have a deep understanding of the tools, work flows, and responsibilities that go into producing production ready software. 

 * We continually push to automate as much as possible.  Fix the process as well as the product.

## We all collectively own everything the team creates

Building a good code infrastructure involves the work of the team, not an individual who feels like the sole proprietor of a project.  Collaboration is key.  Collective ownership allows us to scale up.  Collective ownership allows developers to grow, as subjects are not siloed by certain team members, developers get the opportunity to continually train and learn.

 * You MUST work towards a common convention.  This convention needs to be continually improved upon.  Collectively owning the code increases debate around the convention and allows us to innovate to improve it.

 * We MUST be able to react and adapt to diruptions.

There is a lot more opportunity for people to bring up new frameworks or components (that often overlap and compete with existing ones) without providing adequate support and maintenance.

## We value all of our users and we do the hard work to make the site simple to use

This is for everyone.  Accessible design is good design. Everything we build should be as inclusive, legible and readable as possible.  We’re designing for the whole country, not just the ones who are used to using the web. The people who most need our services are often the people who find them hardest to use. Let’s think about those people from the start.

 * You MUST create accessible, legible and readable experiences.  Use semantically correct markup.  If a user has to click on something, make it a button or a hyperlink.  Use ARIA roles when creating interactions.  Make the page work with a keyboard.  All content should be legible and readable: text must contrast legibly against backgrounds, text must be resizeable and sentences must be written as concisely and understandably as possible.

 * You MUST put user convenience over developer convenience.  Don't push compute tasks down onto the client if you can spend more time creating a server side or offline solution.

 * Making something look simple is easy. Making something simple to use is much harder — especially when the underlying systems are complex — but that’s what we should be doing.

Further reading:

 * [BBC Mobile accessibility guidelines](http://www.bbc.co.uk/guidelines/futuremedia/accessibility/mobile)

## Make things open

We should share what we’re doing whenever we can. With colleagues, with users, with the world. Share code, share designs, share ideas, share intentions, share failures. The more eyes there are on a service the better it gets — howlers are spotted, better alternatives are pointed out, the bar is raised.
Much of what we’re doing is only possible because of open source code and the generosity of the web design community. We should pay that back.