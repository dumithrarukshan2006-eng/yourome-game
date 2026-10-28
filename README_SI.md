# YouroMe — 2D Phone Platformer

මෙය phone browser එකෙන් play කළ හැකි YouroMe 2D fantasy platformer prototype එකකි. HTML Canvas + JavaScript භාවිතා කර ඇත. සාමාන්‍ය prototype එක සඳහා paid game engine එකක් අවශ්‍ය නැහැ.

## දැනට ඇතුළත් දේවල්
- Touch controls: වම/දකුණ, පැනීම, sword attack, magic projectile
- Coin collection, enemies, boss health bar, boss defeat rewards
- Worlds 4ක් සහ boss පරාජය කළ විට unlock වීම
- Coins වලින් sword/magic/health/speed/outfit upgrades
- XP සහ level-up
- Browser `localStorage` save
- Synthesized sound effects, sound toggle
- Phone-size responsive UI

## Phone එකෙන් GitHub Pages publish කරන පියවර
1. GitHub.com වෙත ගොස් sign in කරන්න.
2. `+` → **New repository** තෝරන්න.
3. Repository name එක `yourome-game` ලෙස දාන්න. **Public** තෝරන්න, පසුව **Create repository**.
4. Repository එක තුළ **Add file** → **Upload files** තෝරන්න.
5. ZIP එක extract කරලා එහි ඇතුළත ඇති `index.html` සහ `manifest.webmanifest` file දෙක upload කරන්න. `assets` folder එකත් තිබේ නම් ඒක upload කළ හැකියි. (GitHub website එකෙන් folder upload කිරීම browser අනුව වෙනස් විය හැක.)
6. **Commit changes** ඔබන්න.
7. Repository එකේ **Settings** → **Pages** යන්න.
8. **Build and deployment** යටතේ **Deploy from a branch** තෝරන්න.
9. Branch `main`, folder `/(root)` තෝරා **Save** කරන්න.
10. ටික වේලාවකින් `https://YOUR-USERNAME.github.io/yourome-game/` වැනි URL එකක් ලැබේ. `YOUR-USERNAME` වෙනුවට ඔයාගේ GitHub username එක දාන්න.
11. URL එක phone එකෙන් open කරලා Start Adventure ඔබන්න. Landscape mode එකෙන් වඩා හොඳයි.

## Code එක වෙනස් කරන හැටි
- `index.html` තුළ HTML, CSS සහ JavaScript සියල්ල ඇත.
- Game title / labels වෙනස් කිරීමට HTML කොටස බලන්න.
- World names/colors `worlds` array එකේ ඇත.
- Weapon/shop items `items` array එකේ ඇත.
- Character drawing `drawHero()` function එකෙන් සිදු වේ.
- Enemies `drawEnemy()` සහ `resetWorld()` මගින් සෑදේ.

## Character photos පසුව දාන්නේ කොහොමද?
ඔයාගේ character photo එක upload කළාම, ඒක game character එකට ගැළපෙන sprite/sprite-sheet එකක් ලෙස සකස් කරලා `assets/characters/` තුළ තබන ක්‍රමය සකස් කළ හැකියි. Photo එකේ පසුබිම ඉවත් කිරීම සහ animation frames හදන එක වෙනම asset-editing පියවරක් වෙන්න පුළුවන්. දැන් prototype එක canvas වලින් ඇඳෙන placeholder hero එකක් භාවිතා කරයි.

## වැදගත් සීමා
මෙය සෙල්ලම් කළ හැකි ආරම්භක prototype එකක් — විශාල commercial game එකක් නොවේ. World layouts දැනට procedural/simple; professional character art, polished animations, original music, level maps, save migration සහ performance testing පසුව වැඩිදියුණු කළ හැකියි. Save data එක ඒ browser/device එකේ පමණයි; browser data clear කළොත් නැතිවිය හැකියි. Online multiplayer නැහැ.


## Character art update
The game now loads the custom YouroMe hero sprite art from `assets/characters/` for idle, running, and jumping poses. Keep these four PNG files in the same folder when uploading to GitHub Pages.
