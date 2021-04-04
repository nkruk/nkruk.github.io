---
layout: page
title: About
permalink: /about/
---
# Overcoming the Rails learning swamp with a jurisprudence approach

So you've finished a couple of Ruby on Rails basic courses or even books. For example you may have gone through the [Learn Enough][learn-enough] series and/or Pragmatic's [Agile Web Development with Rails][pragmatic-agile-ruby]. You may have even attempted to create your first [pet project][skiltr] using Rails. Or even browsed extensively through [The Rails Way][the-rails-way] and the outdated yet perennial [Rails AntiPatterns][rails-antipatterns]. And yet, even after going through all those sources, you may feel stuck (I know I do).

It's not the kind of 'stuck' you may suffer with other technologies. Rails will allow you to move along, and implement features/fixes in your own way, even if you only have ugly ways at your disposal. This is exactly what happened to me when I went through my pet project. I stumbled into some roadblocks which I overcame with what I had in my backpack. And the end result, for a while, discouraged me. For example, up until a week ago (March, 2021) I didn't know that I could create a parent model that `accepts_nested_attributes_for` a `has_many` relationship (like a *Project* that has many *Tasks*, or in my case was a *Book excerpt* that had many *Tags* attached to it.) I also didn't know that for something like a tag, or even a comment it's wise to create a polymorphic relationship. So I had to come up with a verbose and non-idiomatic way to achieve my goal. And that's the whole reason I got into Rails in the first place: clean and terse prose that reads as if it were a natural language.

One may reply to me: *It's all on the [official guide][polymorphic-association]*. Yes, that is true. The docs are great if you want to know more about a given specific feature. But there's a long and winding swamp between the gentle land of the basics and [unconscious proficiency][four-stages-of-competence] town. 

Another one may reply: *Just continue creating apps, you'll get it after a while*. That is also true. In fact, that is exactly what I'm attempting at the moment. But I need a new approach. I can't simply follow my previous casual approach. Otherwise I might pick up bad habits and turn Rails into yet another technology that does not make me smile while I use it. A person can get really experienced at using stuff in the wrong way.

Being a swamp dweller myself, I'm in no position to advice what's the best way to get to firm land. But I have set myself the goal to hand out some rope behind me, even if it's just to [affirm newly acquired knowledge][docendo-discimus] (so I provide no guarantees that my rope will lead my fellow mud walkers to safe haven).

The missing link for me is the **use case**. How to solve a given issue or fulfill a spec in a Rails project. Because there's no way I'm reading the references for all the Rails frameworks that I may need to use to implement a given feature. And this is truer for a technology like Rails so attentive to the idea of the [Majestic Monolith][majestic-monolith] in which several frameworks come at work to make something possible. For example, let's go back to my `accepts_nested_attributes_for` case. The implementation for my desired spec required also the creation of a dynamic form which at this point in time it's best if done with [*Stimulus*][stimulus]. And to install *Stimulus* you require to know at least a tiny bit of [*Webpacker*][webpacker]. So the knowledge required didn't stop at something you may find at an 'Advanced *Active Record Associations*' guide. You have to know about *Action View Form Helpers*, *Webpacker*, *Stimulus*, and learn how to add tests to all the involved layers.

It's a fragile path. But there's no simple way around it. I can't know beforehand if there's a better way of doing something and even if I were to become a *book expert* on Rails, that still won't allow me to connect the references to the use cases I may want to tackle with those references.

So that's what I will try to do in this blog. I will share questions I had and the way I answered those questions. I will try to provide concrete and specific examples with the hope that those scenarios could then be translated or generalized to other cases. This is what I like to call the **jurisprudence learning approach**. I would like to gather a collection of use cases wide enough to be translated to similar situations. 

I think this method is very much within the Rails doctrine of [**Convention over configuration**][convention-over-configuration]. What I mean with this is that it's actually highly likely that, as a developer, you'll stumble into a situation like the one I described above where you have a model that `accepts_nested_attributes_for` an associated model. And then, based on that rather probable scenario Rails will present with a convention: handling the association with `accepts_nested_attributes_for` and possibly addind the `inverse_of` option in the relevant `has_many` sentence, and then creating a dynamic form with *Stimulus*. 

The other goal of this blog is of course to keep the conversation open so the community can play the role of a touchstone that will let me know if there's a better way of solving an issue or even if I had made a mistake (which at this point in time, is likely).

In any case, I welcome you to this learning space. Let's put this swamp behind us.

[learn-enough]: https://www.learnenough.com
[pragmatic-agile-ruby]: https://pragprog.com/titles/rails6/agile-web-development-with-rails-6/
[skiltr]: https://skiltr.herokuapp.com/
[the-rails-way]: https://leanpub.com/therails6way
[rails-antipatterns]: https://books.google.es/books/about/Rails_AntiPatterns.html?id=i6mZ0HBDPzsC
[polymorphic-association]: https://guides.rubyonrails.org/association_basics.html#polymorphic-associations
[four-stages-of-competence]: https://en.wikipedia.org/wiki/Four_stages_of_competence
[docendo-discimus]: https://en.wikipedia.org/wiki/Docendo_discimus
[majestic-monolith]: https://m.signalvnoise.com/the-majestic-monolith/
[stimulus]: https://stimulus.hotwire.dev
[webpacker]: https://edgeguides.rubyonrails.org/webpacker.html
[convention-over-configuration]: https://rubyonrails.org/doctrine/#convention-over-configuration