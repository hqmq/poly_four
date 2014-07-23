A little game for me to experiment with [Polymer](http://www.polymer-project.org/).

# What is it?
It is an in-browser implementation of [Score Four](http://en.wikipedia.org/wiki/Score_Four).

<img src="https://cloud.githubusercontent.com/assets/80008/3668631/950e97c4-1221-11e4-9768-215ee0a2496e.png" height="400" />

# Why Did You Make This?
I want to understand the tradeoffs between building a UI with Polymer compared
to a virtual DOM rendering pipeline approach (ie. React and friends).

I assume that there are advantages to both approaches and I am going to explore
the tradeoffs by implementing this little game in both styles.

# Making the demo work
In order for the [demo](http://hqmq.github.io/poly_four/demo.html) to work we
need all of the dependenies (ie polymer and its core components) to be inlined.
That way we don't have to include those bower dependencies into our git repository.

[Vulcanize](https://github.com/Polymer/vulcanize) handles this for us. Whenever
you want to update what is on the demo page, just run the <code>./vulcanize.sh</code>
command which will re-run all of the inlining and generate a new demo.html file.
Then push the new commits to the <code>gh-pages</code> branch.
