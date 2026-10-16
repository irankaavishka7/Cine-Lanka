# Cine-Lanka — වීඩියෝ Player එක භාවිත කරන ආකාරය

මෙය GitHub Pages සඳහා වන static website එකකි. `index.html` තුළ movie details, search, genre filters සහ YouTube privacy-enhanced embedded player එක ඇත.

## GitHub වෙත upload කිරීම

1. GitHub හි ඔබගේ `Cine-Lanka` repository එක විවෘත කරන්න.
2. `index.html` ගොනුව විවෘත කර Edit (පැන්සල්) ඔබන්න. නැතිනම් `Add file` → `Upload files` මගින් ZIP එකෙන් extract කළ `index.html` upload කරන්න.
3. **ZIP ගොනුවම upload නොකරන්න**; ඇතුළේ ඇති `index.html` repository root එකට දමන්න.
4. වෙනස්කම් කළොත් `Commit changes` කරන්න.
5. `Settings` → `Pages` තුළ `main` branch සහ `/(root)` තෝරා තිබේද බලන්න.
6. මිනිත්තු කිහිපයකින් live website එක refresh කරන්න.

## වීඩියෝ ID එකක් එක් කිරීම

`index.html` හි `const movies=[ ... ]` කොටස සොයන්න. Movie එකකට මෙවැනි object එකක් ඇත:

```js
{ id:"my-video", title:"My Video", year:2024, genre:"Drama", rating:"—", image:"", description:"Video description", videoId:"" }
```

YouTube link එක `https://www.youtube.com/watch?v=ABCDEFGHIJK` නම්, `videoId` අගය මෙසේ වෙනස් කරන්න:

```js
videoId:"ABCDEFGHIJK"
```

Video ID එක සාමාන්‍යයෙන් අකුරු/ඉලක්කම්/`_`/`-` වලින් සමන්විත අක්ෂර 11කි. සම්පූර්ණ URL එක නොව ID එක පමණක් යොදන්න.

**වැදගත්:** Embed කිරීමට සහ අවශ්‍ය නම් වාණිජ භාවිතයට අවසර ඇති වීඩියෝ පමණක් එක් කරන්න. YouTube හි `Share` → `Embed` ලබාගත හැකිද බලන්න. සමහර වීඩියෝ embed කිරීම හෝ සමහර රටවල playback සීමා කර තිබිය හැක. Player එක video ID එකක් දාපු පසු පමණක් වීඩියෝව පෙන්වයි; මේ ZIP එකේ demo movies සඳහා video ID හිස්ව තබා ඇත, එබැවින් අනවසර වීඩියෝ කිසිවක් ඇතුළත් කර නැත.

## දෝෂයක් නම්

- GitHub repository root එකේ `index.html` තිබිය යුතුයි.
- `Settings` → `Pages` → `main` / `/(root)` තෝරා තිබිය යුතුයි.
- Commit කළ පසු මිනිත්තු කිහිපයක් ඉඳලා refresh කරන්න.
- Video ID එක හරිද, embed කිරීමට ඉඩ තිබේද බලන්න.
