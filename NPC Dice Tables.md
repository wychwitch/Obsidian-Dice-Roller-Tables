# NPC Dice Table
| dice: 1d4 | Pronouns  |
| --------- | --------- |
| 1         | They/Them |
| 2         | She/Her   |
| 3         | He/Him    |
| 4         | Xe/Xyr    |
^pronouns

| dice: 1d3 | Alignment 1 |
| --------- | ----------- |
| 1         | Chaotic     |
| 2         | Lawful      |
| 3         | Neutral     |
^alignment1

| dice: 1d3 | Alignment 2 |
| --------- | ----------- |
| 1         | Good        |
| 2         | Evil        |
| 3         | Neutral     |
^alignment2

| dice: 1d22 | Goals                             |
| ---------- | --------------------------------- |
| 1          | A better life                     |
| 2          | To Attain Enlightenment           |
| 3          | Attain Infamy                     |
| 4          | Acceptance                        |
| 5          | To Attain Fame                    |
| 5          | To Infiltrate an Opposing Faction |
| 6          | To Acquire a Special Item         |
| 7          | Justice                           |
| 8          | To Craft a Special Item           |
| 9          | Glory                             |
| 10         | To Destroy Special Item           |
| 11         | To Impress Someone                |
| 12         | To Locate Someone                 |
| 13         | To Resolve Dispute                |
| 14         | Love                              |
| 15         | Mastery                           |
| 16         | To Reveal A Secret                |
| 17         | To Serve Their Ideology           |
| 18         | Power                             |
| 19         | Revenge                           |
| 18         | To Serve their Leader             |
| 19         | To Reach A Location               |
| 20         | To Sabotage Opposing Faction      |
| 21         | To Rescue Someone                 |
| 22         | Wealth                            |
^goals

This is weighted to lean more neutral

| dice: 1d110 | Disposition  |
| ----------- | ------------ |
| 1-10        | Loving       |
| 11-20       | Friendly     |
| 21-30       | Helpful      |
| 31-80       | Neutral      |
| 81-90       | Apprehensive |
| 91-100      | Hostile      |
| 101-110     | Violent      |
^disposition

This has equal chances for all dispositions!

| dice: 1d7 | Disposition  |
| ----------- | ------------ |
| 1           | Loving       |
| 2           | Friendly     |
| 3           | Helpful      |
| 4           | Neutral      |
| 5           | Apprehensive |
| 6           | Hostile      |
| 7           | Violent      |
^disposition-alt


| dice: 1d14 | classes      |
| ---------- | ------------ |
| 1          | Barbarian    |
| 2          | Bard         |
| 3          | Cleric       |
| 4          | Druid        |
| 5          | Fighter      |
| 6          | Monk         |
| 7          | Paladin      |
| 8          | Ranger       |
| 9          | Rogue        |
| 10         | Sorcerer     |
| 11         | Warlock      |
| 12         | Wizard       |
| 13         | Artificer    |
| 14         | Blood Hunter |
^class-types

| dice: 1d% | Classes                                                                          |
| -------- | -------------------------------------------------------------------------------- |
| 1-50     | `dice: [[NPC Dice Tables#^class-types]]`                                          |
| 51-100   | `dice: [[NPC Dice Tables#^class-types]]` / `dice: [[NPC Dice Tables#^class-types]]` |
^class


| dice: 1d34 | jobs        |
| ---------- | ----------- |
| 1          | Armorer     |
| 2          | Apothecary  |
| 3          | Artist      |
| 4          | Astrologer  |
| 5          | Baker       |
| 6          | Barber      |
| 7          | Blacksmith  |
| 8          | Bottler     |
| 9          | Butler      |
| 10         | Candlemaker |
| 11         | Carpenter   |
| 12         | Chamberlain |
| 13         | Chancellor  |
| 14         | Clerk       |
| 15         | Clothier    |
| 16         | Constable   |
| 17         | Cook        |
| 18         | Fletcher    |
| 19         | Gardener    |
| 20         | Herbalist   |
| 21         | Jester      |
| 22         | Knight      |
| 23         | Marshal     |
| 24         | Messenger   |
| 25         | Page        |
| 26         | Painter     |
| 27         | Physician   |
| 28         | Potter      |
| 29         | Scribe      |
| 30         | Scholar     |
| 31         | Sheriff     |
| 32         | Shoemaker   |
| 33         | Witch       |
| 34         | Child       | 
^jobs


| dice: 1d4 | Connections                                                |
| --------- | ---------------------------------------------------------- |
| 1         | `dice: [[NPC Dice Tables#^connections-incoming]]`          |
| 2         | `dice: [[NPC Dice Tables#^connections-outgoing]]`          |
| 3         | `dice: [[NPC Dice Tables#^connections-incoming]]` *(secret)* |
| 4         | `dice: [[NPC Dice Tables#^connections-outgoing]]` *(secret)* |
^connections

| dice: 1d5 | Connections-incoming                                                                                                           |
| --------- | ------------------------------------------------------------------------------------------------------------------------------ |
| 1         | `dice: #dnd/npc\|link` helps, aids, or works for them                                                                          |
| 2         | `dice: #dnd/npc\|link` is out to get them                                                                                      |
| 3         | `dice: [[NPC Dice Tables#^connection-npc-or-faction]]` owes them some `dice: [[NPC Dice Tables#^connections-importance]]` debt |
| 4         | `dice: #dnd/npc\|link` is from their past `dice: [[NPC Dice Tables#^connections-opinion]]`                                     |
| 5         | `dice: [[NPC Dice Tables#^connection-npc-or-faction]]` is obstructing their goals (knowingly or unknowingly)                                                   |
^connections-incoming

| dice: 1d9 | Connections-outgoing                                                                                                          |
| --------- | ----------------------------------------------------------------------------------------------------------------------------- |
| 1         | Helps, Aids, or works for `dice: #dnd/npc\|link`                                                                              |
| 2         | They are out to get `dice: #dnd/npc\|link`                                                                                    |
| 3         | They owe `dice: [[NPC Dice Tables#^connection-npc-or-faction]]` some `dice: [[NPC Dice Tables#^connections-importance]]` debt |
| 4         | They are obstructing `dice: [[NPC Dice Tables#^connection-npc-or-faction]]`'s goals (knowingly or unknowingly)                |
| 5         | They're from `dice: #dnd/pc\|link`'s past `dice: [[NPC Dice Tables#^connections-opinion]]`                                    |
| 6         | They know of `dice: #dnd/pc\|link` from rumors `dice: [[NPC Dice Tables#^connections-rumors]]`, `dice: [[NPC Dice Tables#^connections-opinion]]`                               |
| 7         | They know of `dice: #dnd/npc\|link` from rumors `dice: [[NPC Dice Tables#^connections-rumors]]`, `dice: [[NPC Dice Tables#^connections-opinion]]`                              |
| 8         | They are associated with `dice: #dnd/factions\|link`                                                                          |
| 9        | They used to be associated with `dice: #dnd/factions\|link`                                                                   |
^connections-outgoing

| dice: 1d7 | Connections-opinion                                         |
| --------- | ----------------------------------------------------------- |
| 1         | and they are out to get them                                     |
| 2         | and they admire them                                            |
| 3         | and they fear them                                              |
| 4         | and they hate them                                              |
| 5         | and they wish to get closer to them                            |
| 6         | and they personally considers themselves an old friend of theirs |
| 7         | and they remind them of someone dear to them.               |
^connections-opinion

| dice: 1d7 | connections-importance |
| --------- | ---------------------- |
| 1         | piddling               |
| 2         | minor                  |
| 3         | moderate               |
| 4         | considerable           |
| 5         | major                  |
| 6         | great                  |
| 7         | impossible             |
^connections-importance

| dice: 1d2 | connections-rumors   |
| --------- | ------------------ |
| 1         | with truth to them |
| 2         | full of lies       |
^connections-rumors

| dice: 1d2 | npc or faction |
| --------- | ------------------ |
| 1         | `dice: #dnd/npc\|link` |
| 2         | `dice: #dnd/factions\|link`       |
^connection-npc-or-faction

| dice: 1d41 | archetypes|
| --------- | ------------------- |
|1|hero|
|2|anti-hero|
|3|analyst|
|4|bureaucrat|
|5|caretaker|
|6|catalyst|
|7|coward|
|8|curmudgeon|
|9|mentor|
|10|guide|
|11|herald|
|12|trickster|
|13|fool|
|14|innocent|
|15|hermit|
|16|wanderer|
|17|tracker|
|18|judge|
|19|maker|
|20|executioner|
|21|giver|
|22|superhuman|
|23|dreamer|
|24|gossip|
|25|guardian|
|26|hedonist|
|27|leader|
|28|martyr|
|29|everyman|
|30|poet|
|31|rebel|
|32|captive|
|33|samaritan|
|34|scholar|
|35|survivor|
|36|sycophant|
|37|tempter|
|38|tyrant|
|39|sufferer|
|40|ragamuffin|
|41|lackey|
^archetypes


| dice: 1d393 | personal adjective |
| ----------- | ------------------ |
| 1           | able               |
| 2           | abnormal           |
| 3           | absent-minded      |
| 4           | above average      |
| 5           | adventurous        |
| 6           | affectionate       |
| 7           | agile              |
| 8           | agreeable          |
| 9           | alert              |
| 10          | amazing            |
| 11          | ambitious          |
| 12          | amiable            |
| 13          | amusing            |
| 14          | analytical         |
| 15          | angelic            |
| 16          | apathetic          |
| 17          | apprehensive       |
| 18          | ardent             |
| 19          | artificial         |
| 20          | artistic           |
| 21          | assertive          |
| 22          | attentive          |
| 23          | average            |
| 24          | awesome            |
| 25          | awful              |
| 26          | balanced           |
| 27          | beautiful          |
| 28          | below average      |
| 29          | beneficent         |
| 30          | blue               |
| 31          | blunt              |
| 32          | boisterous         |
| 33          | brave              |
| 34          | bright             |
| 35          | brilliant          |
| 36          | buff               |
| 37          | callous            |
| 38          | candid             |
| 39          | cantankerous       |
| 40          | capable            |
| 41          | careful            |
| 42          | careless           |
| 43          | caustic            |
| 44          | cautious           |
| 45          | charming           |
| 46          | childish           |
| 47          | childlike          |
| 48          | cheerful           |
| 49          | chic               |
| 50          | churlish           |
| 51          | circumspect        |
| 52          | civil              |
| 53          | clean              |
| 54          | clever             |
| 55          | clumsy             |
| 56          | coherent           |
| 57          | cold               |
| 58          | competent          |
| 59          | composed           |
| 60          | conceited          |
| 61          | condescending      |
| 62          | confident          |
| 63          | confused           |
| 64          | conscientious      |
| 65          | considerate        |
| 66          | content            |
| 67          | cool               |
| 68          | cool-headed        |
| 69          | cooperative        |
| 70          | cordial            |
| 71          | courageous         |
| 72          | cowardly           |
| 73          | crabby             |
| 74          | crafty             |
| 75          | cranky             |
| 76          | crass              |
| 77          | critical           |
| 78          | cruel              |
| 79          | curious            |
| 80          | cynical            |
| 81          | dainty             |
| 82          | decisive           |
| 83          | deep               |
| 84          | deferential        |
| 85          | deft               |
| 86          | delicate           |
| 87          | demonic            |
| 88          | dependent          |
| 89          | delightful         |
| 90          | demure             |
| 91          | depressed          |
| 92          | devoted            |
| 93          | dextrous           |
| 94          | diligent           |
| 95          | direct             |
| 96          | dirty              |
| 97          | disagreeable       |
| 98          | discerning         |
| 99          | discreet           |
| 100         | disruptive         |
| 101         | distant            |
| 102         | distraught         |
| 103         | distrustful        |
| 104         | dowdy              |
| 105         | dramatic           |
| 106         | dreary             |
| 107         | drowsy             |
| 108         | drugged            |
| 109         | drunk              |
| 110         | dull               |
| 111         | dutiful            |
| 112         | eager              |
| 113         | earnest            |
| 114         | easy-going         |
| 115         | efficient          |
| 116         | egotistical        |
| 117         | elfin              |
| 118         | emotional          |
| 119         | energetic          |
| 120         | enterprising       |
| 121         | enthusiastic       |
| 122         | evasive            |
| 123         | even-tempered      |
| 124         | exacting           |
| 125         | excellent          |
| 126         | excitable          |
| 127         | experienced        |
| 128         | fabulous           |
| 129         | fastidious         |
| 130         | ferocious          |
| 131         | fervent            |
| 132         | fiery              |
| 133         | flabby             |
| 134         | flaky              |
| 135         | flashy             |
| 136         | frank              |
| 137         | friendly           |
| 138         | funny              |
| 139         | fussy              |
| 140         | generous           |
| 141         | gentle             |
| 142         | gloomy             |
| 143         | glutinous          |
| 144         | good               |
| 145         | grave              |
| 146         | great              |
| 147         | groggy             |
| 148         | grouchy            |
| 149         | guarded            |
| 150         | hateful            |
| 151         | hearty             |
| 152         | helpful            |
| 153         | hesitant           |
| 154         | hot-headed         |
| 155         | hypercritical      |
| 156         | hysterical         |
| 157         | idiotic            |
| 158         | idle               |
| 159         | illogical          |
| 160         | imaginative        |
| 161         | immature           |
| 162         | immodest           |
| 163         | impatient          |
| 164         | imperturbable      |
| 165         | impetuous          |
| 166         | impractical        |
| 167         | impressionable     |
| 168         | impressive         |
| 169         | impulsive          |
| 170         | inactive           |
| 171         | incisive           |
| 172         | incompetent        |
| 173         | inconsiderate      |
| 174         | inconsistent       |
| 175         | independent        |
| 176         | indiscreet         |
| 177         | indolent           |
| 178         | indefatigable      |
| 179         | industrious        |
| 180         | inexperienced      |
| 181         | insensitive        |
| 182         | inspiring          |
| 183         | intelligent        |
| 184         | interesting        |
| 185         | intolerant         |
| 186         | inventive          |
| 187         | irascible          |
| 188         | irritable          |
| 189         | irritating         |
| 190         | jocular            |
| 191         | jovial             |
| 192         | joyous             |
| 193         | judgmental         |
| 194         | keen               |
| 195         | kind               |
| 196         | lame               |
| 197         | lazy               |
| 198         | lean               |
| 199         | leery              |
| 200         | lethargic          |
| 201         | level-headed       |
| 202         | listless           |
| 203         | lithe              |
| 204         | lively             |
| 205         | local              |
| 206         | logical            |
| 207         | long-winded        |
| 208         | lovable            |
| 209         | love-lorn          |
| 210         | lovely             |
| 211         | maternal           |
| 212         | mature             |
| 213         | mean               |
| 214         | meddlesome         |
| 215         | mercurial          |
| 216         | methodical         |
| 217         | meticulous         |
| 218         | mild               |
| 219         | miserable          |
| 220         | modest             |
| 221         | moronic            |
| 222         | morose             |
| 223         | motivated          |
| 224         | musical            |
| 225         | naive              |
| 226         | nasty              |
| 227         | natural            |
| 228         | naughty            |
| 229         | negative           |
| 230         | nervous            |
| 231         | noisy              |
| 232         | normal             |
| 233         | nosy               |
| 234         | numb               |
| 235         | obliging           |
| 236         | obnoxious          |
| 237         | old-fashioned      |
| 238         | one-sided          |
| 239         | orderly            |
| 240         | ostentatious       |
| 241         | outgoing           |
| 242         | outspoken          |
| 243         | passionate         |
| 244         | passive            |
| 245         | paternal           |
| 246         | paternalistic      |
| 247         | patient            |
| 248         | peaceful           |
| 249         | peevish            |
| 250         | pensive            |
| 251         | persevering        |
| 252         | persnickety        |
| 253         | petulant           |
| 254         | picky              |
| 255         | plain              |
| 256         | plain-speaking     |
| 257         | playful            |
| 258         | pleasant           |
| 259         | plucky             |
| 260         | polite             |
| 261         | popular            |
| 262         | positive           |
| 263         | powerful           |
| 264         | practical          |
| 265         | prejudiced         |
| 266         | pretty             |
| 267         | proficient         |
| 268         | proud              |
| 269         | provocative        |
| 270         | prudent            |
| 271         | punctual           |
| 272         | quarrelsome        |
| 273         | querulous          |
| 274         | quick              |
| 275         | quick-tempered     |
| 276         | quiet              |
| 277         | realistic          |
| 278         | reassuring         |
| 279         | reclusive          |
| 280         | reliable           |
| 281         | reluctant          |
| 282         | resentful          |
| 283         | reserved           |
| 284         | resigned           |
| 285         | resourceful        |
| 286         | respected          |
| 287         | respectful         |
| 288         | responsible        |
| 289         | restless           |
| 290         | revered            |
| 291         | ridiculous         |
| 292         | sad                |
| 293         | sassy              |
| 294         | saucy              |
| 295         | sedate             |
| 296         | self-assured       |
| 297         | selfish            |
| 298         | sensible           |
| 299         | sensitive          |
| 300         | sentimental        |
| 301         | serene             |
| 302         | serious            |
| 303         | sharp              |
| 304         | short-tempered     |
| 305         | shrewd             |
| 306         | shy                |
| 307         | silly              |
| 308         | sincere            |
| 309         | sleepy             |
| 310         | slight             |
| 311         | sloppy             |
| 312         | slothful           |
| 313         | slovenly           |
| 314         | slow               |
| 315         | smart              |
| 316         | snazzy             |
| 317         | sneering           |
| 318         | snobby             |
| 319         | somber             |
| 320         | sober              |
| 321         | sophisticated      |
| 322         | soulful            |
| 323         | soulless           |
| 324         | sour               |
| 325         | spirited           |
| 326         | spiteful           |
| 327         | stable             |
| 328         | staid              |
| 329         | steady             |
| 330         | stern              |
| 331         | stoic              |
| 332         | striking           |
| 333         | strong             |
| 334         | stupid             |
| 335         | sturdy             |
| 336         | subtle             |
| 337         | sullen             |
| 338         | sulky              |
| 339         | supercilious       |
| 340         | superficial        |
| 341         | surly              |
| 342         | suspicious         |
| 343         | sweet              |
| 344         | tactful            |
| 345         | tactless           |
| 346         | talented           |
| 347         | testy              |
| 348         | thinking           |
| 349         | thoughtful         |
| 350         | thoughtless        |
| 351         | timid              |
| 352         | tired              |
| 353         | tolerant           |
| 354         | touchy             |
| 355         | tranquil           |
| 356         | ugly               |
| 357         | unaffected         |
| 358         | unbalanced         |
| 359         | uncertain          |
| 360         | uncooperative      |
| 361         | undependable       |
| 362         | unemotional        |
| 363         | unfriendly         |
| 364         | unguarded          |
| 365         | unhelpful          |
| 366         | unimaginative      |
| 367         | unmotivated        |
| 368         | unpleasant         |
| 369         | unpopular          |
| 370         | unreliable         |
| 371         | unsophisticated    |
| 372         | unstable           |
| 373         | unsure             |
| 374         | unthinking         |
| 375         | unwilling          |
| 376         | venal              |
| 377         | versatile          |
| 378         | vigilant           |
| 379         | warm               |
| 380         | warmhearted        |
| 381         | wary               |
| 382         | watchful           |
| 383         | weak               |
| 384         | well-behaved       |
| 385         | well-developed     |
| 386         | well-intentioned   |
| 387         | well-respected     |
| 388         | well-rounded       |
| 389         | willing            |
| 390         | wonderful          |
| 391         | volcanic           |
| 392         | vulnerable         |
| 393         | zealous            |
^personal-adj

| dice: 1d120 | Qualities        |
| ----------- | ---------------- |
| 1           | brave            |
| 2           | willing          |
| 3           | determined       |
| 4           | unwilling        |
| 5           | reluctant        |
| 6           | rational         |
| 7           | logical          |
| 8           | obedient         |
| 9           | caring           |
| 10          | healing          |
| 11          | dynamic          |
| 12          | changeable       |
| 13          | mercurial        |
| 14          | unpredictable    |
| 15          | weak             |
| 16          | craven           |
| 17          | fearful          |
| 18          | opinionated      |
| 19          | cranky           |
| 20          | resolute         |
| 21          | educating        |
| 22          | guiding          |
| 23          | helpful          |
| 24          | mystical         |
| 25          | mysterious       |
| 26          | expositional     |
| 27          | revealing        |
| 28          | confusing        |
| 29          | egocentric       |
| 30          | misleading       |
| 31          | clever           |
| 32          | manipulative     |
| 33          | thoughtless      |
| 34          | silly            |
| 35          | amusing          |
| 36          | innocent         |
| 37          | naive            |
| 38          | simple           |
| 39          | straightforward  |
| 40          | credulous        |
| 41          | endearing        |
| 42          | reflecting       |
| 43          | quiet            |
| 44          | secretive        |
| 45          | curious          |
| 46          | curious          |
| 47          | dedicated        |
| 48          | driven           |
| 49          | fair             |
| 50          | unbiased         |
| 51          | patient          |
| 52          | thorough         |
| 53          | crafty           |
| 54          | final            |
| 55          | morbid           |
| 56          | dark             |
| 57          | sombre           |
| 58          | giving           |
| 59          | generous         |
| 60          | charitable       |
| 61          | patronizing      |
| 62          | incredible       |
| 63          | wishful          |
| 64          | ambitious        |
| 65          | talkative        |
| 66          | expositional     |
| 67          | unfettered       |
| 68          | egocentric       |
| 69          | strong           |
| 70          | protective       |
| 71          | egocentric       |
| 72          | short-sighted    |
| 73          | inspiring        |
| 74          | compelling       |
| 75          | self-sacrificing |
| 76          | noble            |
| 77          | common           |
| 78          | typical          |
| 79          | average          |
| 80          | normal           |
| 81          | thoughtful       |
| 82          | lyrical          |
| 83          | myterious        |
| 84          | enlightening     |
| 85          | rebellious       |
| 86          | questioning      |
| 87          | trapped          |
| 88          | abused           |
| 89          | struggling       |
| 90          | angry            |
| 91          | selfless         |
| 92          | generous         |
| 93          | giving           |
| 94          | thoughtful       |
| 95          | curious          |
| 96          | dedicated        |
| 97          | determined       |
| 98          | lucky            |
| 99          | hurt             |
| 100         | predictable      |
| 101         | affirmative      |
| 102         | dependable       |
| 103         | alluring         |
| 104         | deceitful        |
| 105         | dominating       |
| 106         | demanding        |
| 107         | angry            |
| 108         | egocentric       |
| 109         | dedicated        |
| 110         | hurt             |
| 111         | abused           |
| 112         | injured          |
| 113         | fearful          |
| 114         | sickly           |
| 115         | poor             |
| 116         | neglected        |
| 117         | abandoned        |
| 118         | mindless         |
| 119         | devoted          |
| 120         | obedient         |
^qualities
