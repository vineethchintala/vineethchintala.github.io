---
title: "Reading"
---

## Great Reading Experiences

> Craving for a new book is like craving for a new friend - who we expect to have all the qualities of the old ones and still be able to constantly surprise us.

<div class="reads-tabs-container">
    <div class="reads-tabs">
        <button class="reads-tab active" onclick="showCategory('fiction')">FICTION</button>
        <span class="reads-tab-divider">/</span>
        <button class="reads-tab" onclick="showCategory('nonfiction')">NON-FICTION</button>
    </div>
</div>

<div id="fiction-section" class="reads-section active">
    <div class="reading-sidebar">
        <span class="sticky-category">Fiction</span>
    </div>
    <div class="reading-content">
        {{< book title="In Search of lost time" author="Marcel Proust" >}}
        Many writers are good at capturing a particular emotion, a specific moment. Proust gives us not just a snapshot but the full story of a feeling, decoded in a meandering, hypnotic prose.

        Where Proust excels, perhaps more than any other writer I know, is the intensity he brings to everything. There is always something that the narrator is observing so intimately, and so precisely, like a biologist who probes a single type of organism in a series of experiments, though their ultimate goal might be something as universal as understanding the laws of memory, learning or habit.
        {{< /book >}}

        {{< book title="The man without qualities" author="Robert Musil" >}}
        The novel keeps surprising us every time the hero contemplates the boundaries of crime and morality. And every time he observes this boundary, we wonder how he will react to it. Even more, we wonder how he will **define** it. This is the greatness of the book - the cold possibilities for an individual imagined, the equilibrium of society analyzed. Somehow even suicide and murder don't seem to disturb the dusty corners of our minds, as the tension between two best friends or the casual questioning of social values.

        A thinking novel, baked with huge ambition and a creamy layer of lightness. Musil spent the last 20 years of his life writing it and it remains unfinished.
        {{< /book >}}

        {{< book title="Eugene Onegin" author="Alexander Pushkin" >}}
        In my world, this is the best type of novel - short, deep and playful. With exquisite timing, Pushkin can keep you waiting with anticipation, or pass a few comments to make clever transitions that other writers use pages to develop. Eugene Onegin is never boring! (Check out the James Falen translation.)

        The form, the transitions, the range of emotions, the storytelling; There is nothing like it. I delayed submitting my math PhD thesis so that I can include a [poem](/#phd-poem) written in the same rhyme pattern. Vikram Seth, when he was a graduate student in Economics, liked Eugene Onegin so much that he read it five times in one month and went on to write The Golden Gate.
        {{< /book >}}

        {{< book title="Gateway" author="Frederik Pohl" >}}{{< /book >}}

        {{< book title="The Golden Notebook" author="Doris Lessing" >}}{{< /book >}}

        {{< book title="Exhalation" author="Ted Chiang" >}}{{< /book >}}

        <p style="font-style: italic; opacity: 0.85; margin: 2rem 0 1rem 0; font-family: var(--font-main);">19th-century Russian literature, in particular:</p>

        {{< book title="The shot" author="Alexander Pushkin" >}}{{< /book >}}

        {{< book title="Sketches from a hunter's album" author="Ivan Turgenev" >}}{{< /book >}}
    </div>
</div>

<div id="nonfiction-section" class="reads-section">
    <div class="reading-sidebar">
        <span class="sticky-category">Nonfiction</span>
    </div>
    <div class="reading-content">
        {{< book title="Repeat after me" author="David Sedaris" >}}{{< /book >}}

        {{< book title="Hitchcock-Truffaut interviews" >}}{{< /book >}}

        {{< book title="Far from the tree" author="Andrew Solomon" >}}{{< /book >}}

        {{< book title="Consider this" author="Chuck Palahniuk" >}}{{< /book >}}

        {{< book title="The Power Broker" author="Robert Caro" >}}{{< /book >}}

        {{< book title="The Undoing Project" author="Michael Lewis" >}}{{< /book >}}

        {{< book title="Death and life of great American cities" author="Jane Jacobs" >}}{{< /book >}}

        {{< book title="The sensual Quadratic Form" author="John Conway" >}}{{< /book >}}

        {{< book title="Economics" author="Hugh Stretton" >}}{{< /book >}}
    </div>
</div>

<script>
function showCategory(cat) {
    // Toggle active reads-tab button highlight
    document.querySelectorAll('.reads-tab').forEach(btn => {
        const target = btn.getAttribute('onclick');
        if (target && target.includes(cat)) {
            btn.classList.add('active');
        } else {
            btn.classList.remove('active');
        }
    });

    // Toggle active sections display
    document.querySelectorAll('.reads-section').forEach(sec => {
        if (sec.id === cat + '-section') {
            sec.classList.add('active');
        } else {
            sec.classList.remove('active');
        }
    });
}
</script>
