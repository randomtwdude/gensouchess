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
| King   | 4     | Remilia, Alice, Tewi, Joon |
| Queen  | 6     | Reimu, Yukari, Yuuka, Sanae, Koishi, Toyohime |
| Rook   | 7     | Marisa, Patchy, Yuyuko, Reisen, Aya, Suwako, Okuu |
| Bishop | 5     | Kaguya, Eirin, Hina, Orin, Suika |
| Knight | 6     | Sakuya, Youmu, Mokou, Satori, Tenshi, Futo |
| Pawn   | 9     | Cirno, Flan, Mystia, Medicine, Parsee, Seiga, Seija, Lily White, Sunny |

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
Youmu is very good at gardening so she is immune to Yuuka's Blooming Chaos.
