# Gensou Chess design doc
- Chess but there are Touhou pieces.
- There are spells
- Capture pieces to gain spell points to cast them multiple times
- Each side get a few random Touhou pieces.
  - Costs to summon new pieces in game??
- Four player Gensou Chess?

## Touhous

That's enough ideas for a full chaos board!
| Piece  | Count | Characters |
| -----  | ----- | ---------- |
| King   | 4     | Remilia, Alice, Keine, Tewi |
| Queen  | 8     | Reimu, Yukari, Yuuka, Sanae, Koishi, Doremy, Shion, Toyohime |
| Rook   | 7     | Marisa, Patchy, Yuyuko, Reisen, Aya, Suwako, Okuu |
| Bishop | 8     | Kaguya, Eirin, Eiki, Hina, Orin, Suika, Nitori, Mizuchi |
| Knight | 8     | Sakuya, Youmu, Mokou, Satori, Tenshi, Futo, Momoyo, Shinmyoumaru |
| Pawn   | 16    | Cirno, Flan, Mystia, Medicine, Kanako, Parsee, Seiga, Seija, Joon, Kokoro, Sekibanki, Lily White, Aunn, Sunny, Tipsy, Chimata |

### Reimu
- ♟️ Queen

#### Maiden's Grace
When an enemy piece attempts to capture Reimu, there is a `30%` chance that they miss her tiny hitbox and go right past her, the capturing piece and Reimu swap position.
> Random chance in chess let's gooo

#### ᗜnᗜ
Being attacked by any fairy or Tenshi enrages Reimu. An angry Reimu annihilates all opposing pieces she captures.

### Marisa
- ♟️ Rook

#### Master Spark
Marisa fires her signature, totally original and not stolen in any ways, sparkly finisher in any of eight directions, annihilating the first piece it hits. Friendly fire possible!

### Cirno
- ♟️ Pawn
- 🧚 Fairy

#### The Strongest!
Cirno automatically becomes the strongest Queen when she is the only piece you control besides the King.

#### Perfect Freeze
Cirno unleashes an icy storm that freezes all pieces in a 1x3 area (regular movement & capture range of a pawn) in front of her, immobilzing them for `3` turns. Being frozen kills Suwako immediately.

### Patchouli
- ♟️ Rook

#### Mukyu >:(
Running around the board is very tiring! Patchouli has a stamina bar of `15` squares maximum; she regains `2` squares of movement at the end of every move. Capturing an opponent piece replenishes the bar completely.

#### Philosopher's Stone
Patchouli places an elemental marker wherever she goes. The markers are permanent. She may activate Philosopher's Stone when there exists four markers forming a rectangle. The spell is persistent and active for as long as Patchouli is on the board.
All friendly Touhou pieces in the rectangle gains the following effects:
  - All active spells become ready upon invocation of this spell.
  - All spell numerical effects are increased by `1`.
  - Reimu's Maiden's Grace dodge chance is increased to `50%`.

### Sakuya
- ♟️ Knight

#### Luna Dial
When an opposing piece moves, Sakuya can stop time -- and its movement -- dead in their tracks. She may stop the piece at any point along the movement path, which includes preventing the move altogether. A knight move cannot be stopped halfway.
If a knight is stopped, the horse falls to the ground and loses the ability to move for `1` turn.

### Remilia
- ♟️ King

#### Fate of the Blood Moon Night
Fate is in Remilia's favor! She can safely put herself in check; this includes castling into and out of checks. Checks have no effects on the vampire, Remilia must be captured to end the game.

#### Charismatic Cover
The charismatic mistress ducks for cover, granting Remilia the ability to shrug off one capture. The capturer does not move in this case. Each capture by Remilia grants one extra use of this spell, stackable.

### Flandre
- ♟️ Pawn

#### Eye for an Eye
Flandre will not be outdone so easily! When she leaves the board, she removes the perpetrator.

#### Four of a Kind
What's better than Flan? Four Flans! Flandre summons three other Flans around her. The newly summoned Flans do not have initial spell charge.

### Alice
- ♟️ King

#### Seven-Colored Puppeteer
As long as there are pawns on the board, one is randomly selected to be Alice's doll. If the doll is removed from the board, a new one is randomly picked.

#### Rigged!
Alice's dolls are rigged with explosives! She can remotely detonate it, destroying the doll and any piece in the four squares next to it.
Note that Touhou pawns may be chosen as her doll as well, sacrifice with care!

### Yukari
- ♟️ Queen

#### The Gap
Yukari opens a Gap to any empty square on the board. The gap is destroyed if a piece moves onto it. Yukari can choose to teleport to a Gap whenever she likes. After the teleportation, the Gap used is destroyed, and Yukari herself is invulnerable for `1` move.

### Yuyuko
- ♟️ Rook

#### Chaineater
Yuyuko can eat multiple pieces in a single turn, the board is her all-you-can-eat buffet! Yum. Eating Mystia will promote her to a Hungry Queen.

### Youmu
- ♟️ Knight

#### Konpaku
Youmu has two halves and two lives! When Youmu is removed from the board for the first time, she respawns at her starting position; this works even for annihilation.

#### The Gardener
Youmu is very good at gardening and thus immune to Yuuka's Blooming Chaos.

### Mystia
- ♟️ Pawn

#### Song of the Night Sparrow
Any piece that captures her becomes blind. All of your pieces within the movement and capture range of a blind piece is invisible to the opponent.

### Mokou
- ♟️ Knight

#### Eternal Enemies
If Mokou can capture Kaguya, she will do so.

#### Firebird
Mokou is immune to fire.

#### Eternal(ish) Flamewall
Mokou lights the current square on fire. The flame prevents any enemy piece from passing through or moving to it for `5` moves.

### Kaguya
- ♟️ Bishop

#### Eternal Enemies
If Kaguya can capture Mokou, she will do so.

#### Eternal(ish) Moonshine
Kaguya places a barrier on any piece. The barrier protects against fire and from being captured; it is destroyed after `5` moves or after use.

If Mokou is on the board, using this spell lights Kaguya on fire, forcing her to respawn at her starting position unless the barrier is placed on herself.

### Tewi
- ♟️ King

#### Mind of Her Own
Tewi knows all about her prank target. Tewi is immune to being controlled by Reisen.

#### Rabbit Trap
Tewi places an invisible bear trap on any empty square. A piece hit by the trap cannot move for `1` turn. If an opposing piece is captured while trapped, Tewi gains another trap.

### Reisen
- ♟️ Rook

#### Just Another Day
Reisen has gotten good at identifying traps through experience. Reisen is immune to Tewi's tricks.

#### Scarlet Lunacy
Reisen chooses an opposing piece in her movement range and inflicts upon it lunacy which lasts `3` turns. Lunatic pieces may not be controlled and will make random legal moves on its own.

### Eirin
- ♟️ Bishop

#### Help me! Erin!
Erin's Infirmary is capable of bringing back a fallen friend! Respawn it at its starting square.
Pieces annihilated by Angry Reimu, Marisa's Master Spark, Okuu's Second Sun, or Hina's Judgement is beyond even Erin's reach.

### Aya
- ♟️ Rook

#### Bunbunmaru
Aya only spreads the finest information. Designate a move (with a piece type and destination) for your opponent; Aya then publishes it to her newspaper. The move may not be played by your opponent for the rest of the game.

### Yuuka
- ♟️ Queen

#### Blooming Chaos
It's her happy day! A sunflower sprouts at any square within her movement range. If the square is unoccupied, the sunflower blocks it for `2` turns. If the square is occupied, the piece on it is rooted in place and immobilized for `2` turn.

### Eiki
- ♟️ Bishop

#### Prosecution
The entire opposing army is now on trial for multiple offenses against souls. All opposing pieces that are found responsible for killing 3 pieces and above are declared guilty and sentenced to death.
Invisible pieces don't show up at trials and are exempt.

### Medicine
- ♟️ Pawn

#### Lovely Poison
At the start of your turn, all opposing pieces immediately surrounding Medicine become poisoned.
If, at any moment, three or more poisoned pieces occupy any 2x2 area, all of them suffer heart attacks and die on the spot.

### Kanako
- ♟️ Pawn

#### High Wind God
The weather is crazy out there. The wind pushes the pieces in front of Kanako, in her file and to its left and right, back `2` squares. Pieces are destroyed if the movement is otherwise impossible.

### Suwako
- ♟️ Rook
- 🐸 Frog

#### Flycatcher
Suwako spits her tongue out in any of four cardinal directions, catching the first piece in the way and pulling it back next to her. The caught piece is destroyed if the movement is otherwise impossible.
Suwako cannot catch pieces frozen by Cirno.

### Sanae
- ♟️ Queen

#### Face Off
Sanae wants blood and your faith! For `5` turns, Sanae turns into a Rook but can move twice in a turn, smashing through the lines recklessly. If Sanae fails to capture at least nine points worth of material during the time, she is given a stern talking to
by Kanako and permanently demoted to a Rook.

Opposing Reimu's spells are disabled for the duration, she better watch out!

### Keine
- ♟️ King

#### Ahistoric
Move history is hidden from your opponent.

#### Foggy Past
Keine erases the opponent's recollection of your position. All squares not within the opponent's movement range become invisible to them just like in Fog of War; however, once the fog on one square is cleared once, it remains clear.

### Hina
- ♟️ Bishop

#### Judgement
Hina bears the suffering for all her friends, hoping for a better future without her. All negative effects of all your pieces are cleansed, they also gain immunity to all negative effects for `3` turns, Hina is annihilated.

### Parsee
- ♟️ Pawn

#### Hashihime
The hashihime will let only the good pass. All friendly pieces' movements and spells may pass through her bridge and behave as if she was not obstructing.

### Okuu
- ♟️ Rook

#### Second Sun
This spell may be cast after making a move.

Okuu prepares a small thermonuclear bomb. The charging takes two turns, during which Okuu cannot move. The bomb may be cancelled by herself or by destroying or freezing her. If Okuu cancels the bomb herself, the spell cost is refunded.
Upon detonation, the closest pieces to her in all eight directions, up to two squares or one diagonal away, are annihilated. The detonation happens before your move.

### Orin
- ♟️ Bishop

#### Soul Collector
Orin goes to work collecting the souls of the opponent's pieces, bringing them back into the fight on your side. Choose one captured and non-annihilated opposing piece to respawn on any empty square on your side of the board.

### Koishi
- ♟️ Queen

#### Unconcious Requiem
Koishi is invisible to your opponent until she makes her first capture. If she manages to backstab the victim (the capturing move is made towards your side of the board), Koishi remains undectected. Watch your back!

### Satori
- ♟️ Knight

#### Satori Link
Only Satori has some vague idea of where her sister is. Satori shows you roughly where an opposing Koishi is relative to her.

#### The Third Eye
Satori reads the opponent's mind and sees a move...

Designate a move (with a piece type and destination) for your opponent; if it is legal now, they must play it within three moves or lose.

### Doremy
- ♟️ Queen

#### U r my dream
Descend into your dream world... For `3` turns, all of your non-pawn pieces move like Queens! After the dream is over, the board returns to the state before this spell is cast.

### Seiga
- ♟️ Pawn

#### Unbound
Seiga can move forward through any number of pieces. She can promote from this. This spell is only available for Pawn Seiga.

### Seija
- ♟️ Pawn

#### Flipped World
Seija can move (but not capture) backwards. She can also en passant multiple times.

### Tenshi
- ♟️ Knight

#### The word that starts with an M
Tenshi is immune to fire. Every time she is targeted by a negative effect, Tenshi gains one spell point. Being rooted by Yuuka's flower grants one extra spell point.
> This is perfectly normal interaction

#### Seismo
Tenshi messes around and causes an earthquake! The earthquake has a `?` chance to rupture any square, immobilzing the piece on it for `1` turns. The more spell points Tenshi has when casting Seismo, the higher the chance will be.

Reimu will be immobilized for `1` extra turn by this spell; its use, whether or not it actually affects Reimu, enrages the shrine maiden.

### Joon
- ♟️ Pawn

#### Divestment
Joon compels both players to play recklessly and wastefully. For the next `3` turns, capturing is mandatory if possible for both sides.

### Shion
- ♟️ Queen

#### Mutual Misfortune
The player which controls more material must give up their pieces such that they no longer have the material advantage.

### Kokoro
- ♟️ Pawn

#### Sad Mask
Kokoro selects any piece excluding the King within her movement and capture range and forces it to have cripplingly low self-esteem. The piece is now really, really sad and it must capture any piece within three moves to validate its worth; otherwise it will leave the board in sadness.

### Suika
- ♟️ Bishop

#### Misty Split
In addition to the original square she is on, select two empty squares on the board. In a puff of (likely alcoholic) mist, Suika disappears and re-emerges as three mini-Suikas at the chosen squares.

Only one is the real Suika, she will be at one of the three squares chosen by you, her identity is only known to you. Only the real Suika may capture and cast spells.

### Sekibanki
- ♟️ Pawn

#### Detached HEAD state
Capturing a piece sets Sekibanki into detached HEAD state, she simply spawns a new Banki at the captured square. The original Banki cannot cast this spell again.

### Futo
- ♟️ Knight

#### The Art of Arson
At the start of your turn, Futo sets opposing pieces immediately surrounding her on fire. The fire lasts `2` turns and can be refreshed. If a piece is on fire for five turns in a row, it is destroyed.

### Lily White
- ♟️ Pawn
- 🧚 Fairy

#### Haru-binger
The gentle breeze of spring cleanses negative effects of friendly pieces immediately around her every other turn.

### Aunn
- ♟️ Pawn

#### En Garde
Aunn can choose to become the stone guardian of the Shrine or return to her moving state at any time. While Aunn is acting as a guardian, she cannot move, be captured, is immune to negative effects and explosions.

### Momoyo
- ♟️ Knight

#### Blast Protection enchantment.level.255
She claims it's fully survival. Whichever case it may be, Momoyo is immune to explosions. Master Sparks are not explosions.

#### Dynamite
Momoyo digs a hole and hides a TNT in it. She can detonate the TNT if she later comes back to the square. Momoyo can put down multiple TNT and they will all detonate at once. The explosions kill the piece occupying the square.

### Shinmyoumaru
- ♟️ Knight

#### BONK
That's it! I'm gettin' me mallet! Shinmyoumaru can swing her Miracle Mallet anywhere she can move to, making her foes small for `3` turns. Small pieces move and capture like pawns but may not en passant.

### Sunny
- ♟️ Pawn
- 🧚 Fairy

#### Sore sore sore sore!
When Sunny has advanced past the fourth rank and is not being attacked by any opposing pieces, she secretly calls in her partner in crime -- Luna Child! The piece is transformed into Sunny & Luna.

#### Soyya soyya soyya soyya!
When Sunny & Luna has advanced past the fifth rank and is not being attacked by any opposing pieces, they secretly call in their partner in crime -- Star Sapphire! The piece is transformed into The Three Fairies.
Using this spell enrages Reimu.

#### Great Fairy War
The Three Fairies together make the dream work! Become a Queen immediately.

If you control at least one other fairy, target an opposing Queen with a big prank, immobolizing it for `3` turns.

### Toyohime
- ♟️ Queen

#### Simply Connected
With a light wave of her fan, Toyohime connects the left and right sides of the board, allowing her to move off the board and wrap back around in a single move.

#### Fully Connected
For `3` turns, every single one of your pieces enjoy the same powers as Toyohime herself.

### Nitori
- ♟️ Bishop

#### Remote Control
The Kappa Industries (tm) Remote Control Apparatus (tm) allows Nitori to control another piece for you. Nitori can install the Remote Control on any friendly piece within her movement range. Whenever Nitori is to move, the piece with Remote Control installed can be moved as well, after Nitori.

The Remote Control Apparatus has a charge of 5 uses. Every capture by Nitori recharges it by one use.

### Tipsy
- ♟️ Pawn
- 🧚 Fairy

#### Ballistic Fairy
When a Queen is next to Tipsy, they can choose to launch her in any of eight directions. The Ballistic Tipsy has a maximum range of 4 squares or 3 diagonals, if she strikes a piece, the target is destroyed while Tipsy herself is stunned for `3` moves.
When Tipsy is fired by Reimu, there is no range restrictions and target struck is annihilated.
A Ballistic Tipsy will be blocked by and stop in front of an invulnerable target.

> Jo2n's cute fairy

### Chimata
- ♟️ Pawn

#### Return To Nothing
Chimata forces your opponent to pick a piece they control to give up. The piece given up becomes neutral and is capturable.

### Mizuchi
- ♟️ Bishop

#### Possession
Mizuchi selects a piece within her movement range to possess for `2` turns, gaining full control over it. The possession is cancelled if Mizuchi moves or is otherwise attacked by any means.
