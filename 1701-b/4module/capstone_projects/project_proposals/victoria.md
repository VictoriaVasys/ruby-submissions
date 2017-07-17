## Pocket Plants

### Pitch

Ever been on a plant walk, a forest hike, or even just a little jaunt through your neighborhood and thought, wow, that's a gorgeous flower! I wish I could have that in my front yard! Or, that looks super weird! I wonder what it is. Or, I think I've seen that before, I wonder if it's invasive. Never fear, pocket plants is here!


### Problem

Friends and I often wonder what plants we're looking at, both when walking through the neighborhood & out on a nature walk. I want to know whether the species is non-invasive, native, and has beneficial properties (attracts good insects, deters bad ones, has a tap root to draw up nutrients, is disease-resistant, etc.), and if so, how I could grow it at home!

### Solution

I'll use the Google Cloud Vision API to try to recognize the plant (I tried this weekend with 2 photos & one worked! I think if the photo is birds-eye view, it should have a better time finding a match). If there's pretty good confidence with the name (>50%?), I'll target another API (there's a taxonomy one, but didn't have time to dig in too far) to gather information about 1. invasiveness, 2. native-ness 3. growing information & 4. companion planting ideas (if I get there). I'd also like to build a database with common plants & info.

### Target Audience

This would be applicable to anyone who's curious about plants! Whether you're a home gardener, a farmer who is new to wild plants, or just the average person who loves plants, this app is for you!

### New Techniques

I'll be building a react front-end, implementing Rails loggers, seeding a giant db to test that my SQL is up-to-standard, and I'd like to implement background-workers somehow but haven't come up with a good use-case for them yet.

### Workflow

I haven't fully decided yet, but either Kanbachi, Jira, Asana, or Trello.
