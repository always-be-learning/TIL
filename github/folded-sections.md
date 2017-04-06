# Folded sections in your markdown docs

Sooo, this is pretty sweet! If you wrap a long section of… whatever in `<details>…</details>` you can create a folded section in your document on the fly. Super useful for stack traces, output, etc., etc.

Add `<summary>description</summary>` and your folded section will have the title of your choice. 🙂

<details>
<summary>The Second Coming by William Butler Yeats</summary>

    Turning and turning in the widening gyre
    The falcon cannot hear the falconer;
    Things fall apart; the centre cannot hold;
    Mere anarchy is loosed upon the world,
    The blood-dimmed tide is loosed, and everywhere
    The ceremony of innocence is drowned;
    The best lack all conviction, while the worst
    Are full of passionate intensity.

    Surely some revelation is at hand;
    Surely the Second Coming is at hand.
    The Second Coming! Hardly are those words out
    When a vast image out of Spiritus Mundi
    Troubles my sight: a waste of desert sand;
    A shape with lion body and the head of a man,
    A gaze blank and pitiless as the sun,
    Is moving its slow thighs, while all about it
    Wind shadows of the indignant desert birds.

    The darkness drops again but now I know
    That twenty centuries of stony sleep
    Were vexed to nightmare by a rocking cradle,
    And what rough beast, its hour come round at last,
    Slouches towards Bethlehem to be born?

</details>


## Notes

Found `<details>` and `<kbd>` [via Twitter](https://twitter.com/felixrieseberg/status/849082760098709506)

### formatting…

I used multiple `<details>` sections in an Issue, today, and learned that stacked `<details>` sections with code blocks in them want 2 blank lines in between them, or they won't all render correctly
